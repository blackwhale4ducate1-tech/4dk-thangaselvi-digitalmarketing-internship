# Google Ads Campaign Hierarchy & Account Structure

## 🎯 1. Purpose & Business Context
A well-structured Google Ads account is essential for managing budgets, quality scores, and conversion tracking. Grouping unrelated keywords into a single campaign makes it difficult to control budgets or direct traffic to targeted landing pages.

This document outlines the **Campaign Hierarchy** for our Online Fitness Coaching business. We use a structured system split by search intent: Brand Protection, Competitor Conquest, Service/Intent Search, and Audience Remarketing. This ensures that every keyword is matched with a highly relevant ad group, ad copy, and landing page.

---

## 📂 2. Account Hierarchy & Budget Settings

Our account structure is built as follows:

```text
  GOOGLE ADS ACCOUNT
  ├── [CAMPAIGN 01] BRAND PROTECTION (10% Budget)
  │    └── [AD GROUP 01] Brand Core (Keywords: [FitLife Coaching], etc.)
  │
  ├── [CAMPAIGN 02] COMPETITOR CONQUEST (20% Budget)
  │    ├── [AD GROUP 01] App Competitors (Future, CoPilot)
  │    └── [AD GROUP 02] Service Competitors (Caliber, Kickoff)
  │
  ├── [CAMPAIGN 03] SERVICE & INTENT (55% Budget)
  │    ├── [AD GROUP 01] General Coaching ("online fitness coach", etc.)
  │    ├── [AD GROUP 02] 1-on-1 Personal Training ("remote personal trainer", etc.)
  │    └── [AD GROUP 03] Nutrition & Custom Diets ("diet coaching online", etc.)
  │
  └── [CAMPAIGN 04] REMARKETING DISPLAY (15% Budget)
       ├── [AD GROUP 01] Website Visitors (Retargeting list - 30 days)
       └── [AD GROUP 02] Lead Form Dropouts (Retargeting list - 60 days)
```

### Campaign Structure Matrix
| Campaign Name | Targeting Strategy | Bidding Model | Target KPI |
| :--- | :--- | :--- | :--- |
| **01. Brand Protection** | Exact brand search terms. | Target Impression Share (95% Top of Page) | **Impression Share > 90%** |
| **02. Competitor Conquest** | Competitor brand names. | Manual CPC (Bid high) | **Ad Position 1-3** |
| **03. Service & Intent** | Phrase/Exact category keywords. | Maximize Conversions (Target CPA: $50) | **Conversion Rate > 3%** |
| **04. Remarketing** | Custom retargeting lists. | Maximize Conversions | **Cost Per Lead < $40** |

---

## 🛠️ 3. Step-by-Step Settings Configuration

1.  **Geography & Location Settings:** Set location settings to "Presence: People in or regularly in your targeted locations" (do not use "Presence or Interest", which can trigger international spam traffic). Target US/UK/CA.
2.  **Language Settings:** Set target language to English.
3.  **Ad Rotation:** Set ad rotation settings to **Optimize: Prefer best performing ads** (allows Google to favor higher-CTR ad copy variations).
4.  **Search Partners and Display Network:** Uncheck both "Include Google search partners" and "Include Google Display Network" on search campaigns to prevent low-intent clicks. (Remarketing Campaign 04 is the only campaign allowed on the Display Network).

---

## 🖼️ 4. Example Screenshot Descriptions
*   **Screenshot 1: Campaign Network Target Toggles**
    *   *Description:* A screen view of Google Ads Campaign settings showing the "Search Network" and "Display Network" checkboxes under the Networks panel. Red arrows point to both checkboxes unchecked with a callout warning against automated display expansion.
*   **Screenshot 2: Audience Segment Manager for Remarketing**
    *   *Description:* The Google Ads Audience Manager page showing custom segments. It highlights lists for "All Website Visitors (30 Days)" and "Lead Form Submissions (Excluded)" to show how to structure target segments.

---

## 🚫 5. Common Mistakes to Avoid
*   **Mixing Search and Display Networks:** Enabling Display Network on a Search Campaign. This wastes budget on low-CTR display ads and skews search metrics.
*   **Leaving Location Settings on Default:** Using the default "Presence or Interest" targeting. This allows people searching from outside your target countries to see and click your ads.
*   **Bidding on Brand Keywords in Service Campaigns:** Bidding on brand keywords inside your non-brand campaigns. This inflates non-brand metrics and makes it difficult to track brand protection performance.

---

## 📅 6. Expected Outcomes & Timelines
*   **Day 1:** Build the campaign structure inside Google Ads Editor.
*   **Day 2:** Configure campaign-level settings (budgets, bidding models, geographic targets).
*   **Day 4:** Launch campaigns in paused status for tracking verification.
*   **Expected Outcome:** A clean, organized account structure that makes budget management and performance reporting straightforward.
