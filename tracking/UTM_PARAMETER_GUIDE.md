# Google Ads UTM Tracking & ValueTrack Guide

## 🎯 1. Purpose & Business Context
UTM (Urchin Tracking Module) parameters are tags added to the end of URLs to identify traffic sources inside web analytics platforms (like Google Analytics 4) and CRM systems (like HubSpot or Salesforce).

This guide outlines our standard **UTM Naming Convention** and details how to implement Google Ads **ValueTrack Parameters** to dynamically pull campaign, ad group, match type, and keyword data directly into our CRM. This tracking helps us measure lead quality and close rates back to individual search terms.

---

## 📋 2. UTM Tracking Template Specification

We use a standardized tracking template applied at the Google Ads **Account Level**. This automatically applies tracking tags to all active campaigns.

### The Tracking Template
```text
{lpurl}?utm_source=google&utm_medium=cpc&utm_campaign={_campaignname}&utm_adgroup={adgroupid}&utm_content={creative}&utm_term={keyword}&matchtype={matchtype}&device={device}&network={network}
```

### Parameter Breakdown & Definitions
| UTM Parameter | Google Ads Dynamic Tag | Example Output Value | Definition |
| :--- | :--- | :--- | :--- |
| **utm_source** | `google` (Hardcoded) | `google` | Identifies the traffic source. |
| **utm_medium** | `cpc` (Hardcoded) | `cpc` | Identifies the traffic channel. |
| **utm_campaign**| `{_campaignname}` (Custom Parameter) | `03_Search_Service_US` | Identifies the active campaign. |
| **utm_adgroup** | `{adgroupid}` (ValueTrack Tag) | `1234567890` | Pulls the unique Google Ad Group ID. |
| **utm_content** | `{creative}` (ValueTrack Tag) | `9876543210` | Pulls the unique Ad ID. |
| **utm_term** | `{keyword}` (ValueTrack Tag) | `online fitness coach` | Pulls the target search keyword. |
| **matchtype** | `{matchtype}` (ValueTrack Tag) | `e` (exact) or `p` (phrase) | Identifies the keyword match type. |
| **device** | `{device}` (ValueTrack Tag) | `m` (mobile) or `c` (desktop) | Identifies the user's device. |
| **network** | `{network}` (ValueTrack Tag) | `g` (google search) | Identifies the search network. |

---

## 🛠️ 3. Step-by-Step Implementation Instructions

1.  **Configure Account Tracking Template:**
    *   Log in to Google Ads. Navigate to **Settings > Account Settings**.
    *   Click the **Tracking** accordion menu.
    *   In the **Tracking template** field, paste the tracking template code block exactly as written above.
2.  **Define Custom Campaign Parameter:**
    *   Because Google's default campaign ID tag (`{campaignid}`) outputs a string of numbers rather than a campaign name, we use a custom parameter.
    *   Go to your campaign settings. Under **Campaign URL options**, define a custom parameter named `_campaignname` and set the value to your descriptive campaign name (e.g., `03_Search_Service_US`).
3.  **Verify Tracking Links:**
    *   In the Tracking setup panel, click the **Test** button.
    *   Google will test your landing page links with the parameters applied. Verify that all test URLs return a green **200 OK** checkmark (indicating the parameters do not cause 404 page errors).

---

## 🖼️ 4. Example Screenshot Descriptions
*   **Screenshot 1: Account Settings Tracking Panel**
    *   *Description:* A screenshot of the Account Settings dashboard in Google Ads. The Tracking accordion is open, showing the Tracking template field filled out with a red highlight box around the ValueTrack tags.
*   **Screenshot 2: URL Tracking Options Test Results**
    *   *Description:* The tracking verification pop-up window in Google Ads displaying test results. A list of landing page URLs is shown, with a column displaying green checkmarks and "Landing page found" messages.

---

## 🚫 5. Common Mistakes to Avoid
*   **Mixing Case in UTM Values:** Writing `utm_source=Google` in one campaign and `utm_source=google` in another. GA4 parses these as separate traffic sources. Always use **lowercase** for hardcoded UTM parameters.
*   **Hardcoding Search Keywords:** Hardcoding search terms in tracking links (e.g. `utm_term=fitness`). This outputs the same keyword value for all clicks; always use the dynamic `{keyword}` ValueTrack parameter.
*   **Not Testing Redirects:** Applying parameters to sites that remove query parameters during redirects. Test your tracking template to verify that your CMS retains the UTM values on landing pages.

---

## 📅 6. Expected Outcomes & Timelines
*   **Implementation:** Configure the account tracking template during initial account setup (Day 3).
*   **Expected Results:** 100% of organic clicks tracked, passing campaign and keyword metrics directly into GA4 and CRM platforms from launch.
