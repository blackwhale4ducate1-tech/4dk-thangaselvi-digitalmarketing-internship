# Google Ads Conversion Tracking & Google Tag Manager Setup

## 🎯 1. Purpose & Business Context
Conversion tracking is essential for measuring PPC performance. Without accurate conversion tracking, we cannot tell which keywords lead to trial sign-ups or strategy bookings, and Google's Smart Bidding algorithms will not function.

This document outlines how to configure **Google Tag Manager (GTM)** to track three core conversion actions: Lead Form Submissions, Coaching Subscription Purchases, and Phone Link Clicks. It also explains why we use the **Data-Driven Attribution** model to optimize performance.

---

## 📋 2. Core Conversion Actions & GTM Configuration

### A. Conversion Action 1: Lead Form Submission (Free Strategy Call)
*   **Conversion Name in Google Ads:** `Lead - Strategy Call Booked`
*   **Trigger Type:** Page View
*   **Trigger Rule:** Page URL contains `/thank-you` (the redirection landing page reached only after form submission).
*   **GTM Configuration:**
    1.  **Trigger:** Create a page-view trigger named `Pageview - Thank You Page`. Set rule: `Page URL contains /thank-you`.
    2.  **Tag:** Create a Google Ads Conversion Tracking tag. Input your Conversion ID and Conversion Label. Assign the trigger to fire this tag.

### B. Conversion Action 2: Premium Purchase (Coaching Signup)
*   **Conversion Name in Google Ads:** `Purchase - Subscription Completed`
*   **Trigger Type:** Custom Event (via Data Layer)
*   **Trigger Rule:** Event name equals `purchase`.
*   **GTM Configuration:**
    1.  **Trigger:** Create a Custom Event trigger named `Custom Event - Purchase`. Set event name to `purchase`.
    2.  **Tag:** Create a Google Ads Conversion Tracking tag. Pull purchase value and currency code using GTM variables (e.g. `{{DLV - Purchase Value}}`, `{{DLV - Currency}}`) to pass transaction values back to Google Ads.

### C. Conversion Action 3: Click-to-Call (Phone Clicks)
*   **Conversion Name in Google Ads:** `Click - Phone Link`
*   **Trigger Type:** Just Links
*   **Trigger Rule:** Click URL starts with `tel:`.
*   **GTM Configuration:**
    1.  **Trigger:** Create a trigger named `Link Click - Phone`. Set rule: `Click URL starts with tel:`.
    2.  **Tag:** Create a Google Ads Conversion Tracking tag to register phone click conversions.

---

## ⚖️ 3. Attribution Model Selection: Data-Driven Attribution (DDA)
We configure all conversion actions inside Google Ads to use the **Data-Driven Attribution** model:
*   **Why it works:** Unlike outdated models (like Last-Click or First-Click), Data-Driven attribution uses account history data to distribute conversion credit across all touchpoints (e.g. user clicks competitor ad first, then returns via service campaign, and finally converts via remarketing).
*   **Business Outcome:** Provides a realistic view of how top-of-funnel keyword campaigns contribute to conversions, preventing the team from pausing keywords that assist conversions.

---

## 🛠️ 4. Step-by-Step GTM Implementation Guide

1.  **Install the Conversion Linker:** 
    *   In GTM, create a new tag.
    *   Select **Conversion Linker** as the tag type.
    *   Set the trigger to **All Pages** (this tag is required for accurate tracking on modern browsers).
2.  **Configure Google Ads Tags:**
    *   Create tags for Form Submissions, Purchases, and Phone Clicks.
    *   Input your conversion details (ID and labels) from Google Ads.
3.  **Preview and Test:**
    *   Click **Preview** in GTM to launch GTM Debug mode.
    *   Complete a test form submission on your landing page.
    *   Verify that your `Lead - Strategy Call Booked` tag fires successfully.
4.  **Publish Container:** Click **Submit** and publish your GTM container container workspace.

---

## 🖼️ 5. Example Screenshot Descriptions
*   **Screenshot 1: GTM Trigger Configuration Panel**
    *   *Description:* A screen view of Google Tag Manager displaying a Custom Event trigger named "Custom Event - Purchase". The event name is set to "purchase", and it is configured to fire on "All Custom Events".
*   **Screenshot 2: Google Ads Conversion Settings**
    *   *Description:* The conversion details page in Google Ads for "Lead - Strategy Call Booked". The settings display "Primary action (used for bidding optimization)" and "Attribution model" set to "Data-driven".

---

## 🚫 6. Common Mistakes to Avoid
*   **Missing the Conversion Linker Tag:** Forgetting to implement the Conversion Linker tag. This prevents tracking tags from saving conversion cookies, leading to under-reported conversions on mobile devices.
*   **Double-Counting Conversions:** Setting your lead form submission conversion to count "Every" conversion instead of "One". If a user refreshes the thank-you page multiple times, it will register as multiple leads, inflating conversion metrics. Set count settings to "One" for lead actions.
*   **Bypassing Preview Mode Testing:** Publishing GTM containers without verifying tags in preview mode first. This can result in broken tracking codes going live and a loss of conversion data.

---

## 📅 7. Expected Outcomes & Timelines
*   **Tracking Setup:** Deploy GTM tags and verify conversion tracking on Day 3.
*   **Expected Results:** 100% accurate conversion tracking, matching leads and sales back to the keyword and ad level within 24 hours of launch.
