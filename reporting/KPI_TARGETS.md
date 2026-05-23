# Google Ads PPC KPI Targets & Performance Benchmarks

## 🎯 1. Purpose & Business Context
Measuring PPC campaign health requires clear, quantifiable targets. Without performance benchmarks, campaign optimizations can feel subjective and budget performance is difficult to measure.

This document defines our **Key Performance Indicator (KPI) Targets** for our Online Fitness Coaching campaigns. It provides the calculation formulas for each metric and outlines the action thresholds that trigger optimization reviews if performance falls below target benchmarks.

---

## 📋 2. Core PPC KPI Targets

### A. Click-Through Rate (CTR)
*   **Target Benchmark:** **>5.0%** (for core Search campaigns).
*   **Formula:** $\text{CTR} = (\text{Clicks} / \text{Impressions}) \times 100$
*   **Action Threshold:** If CTR falls below **3.0%** on core service campaigns, trigger a review of ad copy headlines, match types, and negative keywords.

### B. Quality Score
*   **Target Benchmark:** **>7/10** (across core service keywords).
*   **Components:** Expected CTR, Ad Relevance, and Landing Page Experience.
*   **Action Threshold:** If Quality Score falls below **5/10** on a high-traffic keyword, check landing page speed, optimize H-tags, and ensure the keyword appears in your ad copy headlines.

### C. Landing Page Conversion Rate (CVR)
*   **Target Benchmark:** **>3.0%** (percentage of visitors booking a strategy call).
*   **Formula:** $\text{CVR} = (\text{Conversions} / \text{Clicks}) \times 100$
*   **Action Threshold:** If CVR falls below **1.5%**, run a CRO audit of the landing page using the [CRO_CHECKLIST.md](file:///d:/4DK/Projects/Marketting/google-ads-ppc-fitness/landing-pages/CRO_CHECKLIST.md) (e.g., check mobile forms, above-the-fold elements, and load speeds).

### D. Cost Per Acquisition (CPA)
*   **Target Benchmark:** **$50.00** per booked call.
*   **Formula:** $\text{CPA} = \text{Total Ad Cost} / \text{Conversions}$
*   **Action Threshold:** If CPA exceeds **$75.00** over a 7-day period, review keyword bids, check search terms reports for wasted spend, and audit landing page conversion paths.

### E. Return on Ad Spend (ROAS)
*   **Target Benchmark:** **3.0x** (based on a 3-month Customer Value baseline of $450).
*   **Formula:** $\text{ROAS} = \text{Coaching Revenue Generated} / \text{Ad Spend}$
*   **Action Threshold:** If ROAS falls below **2.0x**, verify phone close rates with sales teams and audit campaign keyword quality.

---

## 🛠️ 3. Step-by-Step Reporting SOP

1.  **Select Date Parameters:** Set your reporting view to the last **7 days** or **30 days** in Google Ads.
2.  **Add Metric Columns:** Go to **Columns > Modify Columns**. Add columns for `CTR`, `Quality Score`, `Cost / conv.` (CPA), and `Conv. rate`.
3.  **Evaluate Performance:** Compare the columns against the target benchmarks listed above.
4.  **Triage Underperforming Elements:** If any metric falls below its action threshold, log an action item in your weekly report to optimize it.

---

## 🖼️ 4. Example Screenshot Descriptions
*   **Screenshot 1: Quality Score Diagnostics in Google Ads**
    *   *Description:* A screen view of the Google Ads keyword panel showing the Quality Score column. High-traffic keywords are displayed, with a callout bubble open displaying diagnostics for "Expected CTR (Above Average)", "Ad Relevance (Above Average)", and "Landing Page Experience (Average)".
*   **Screenshot 2: Conversion Metrics Report Dashboard**
    *   *Description:* A Google Ads custom dashboard page showing scorecards for CTR (5.6%), average CPA ($48.50), and conversion rate (3.8%) in green cards indicating target levels are met.

---

## 🚫 5. Common Mistakes to Avoid
*   **Optimizing CTR at the Expense of CPA:** Writing clickbait ad headlines that increase clicks but don't convert on the landing page. This inflates CTR metrics while increasing CPA. Focus ad copy on your specific offer.
*   **Ignoring the Learning Phase:** Judging campaign CPAs during the initial 7-14 day Smart Bidding learning phase. Let the algorithm complete its learning cycle before analyzing CPA metrics.
*   **Comparing Brand vs. Service CPA Directly:** Expecting competitor conquest or service search campaigns to achieve the same low CPA ($10-$20) as brand protection campaigns. Evaluate campaigns against their specific targets.

---

## 📅 6. Expected Outcomes & Timelines
*   **Initial Review:** Complete the first performance checkup 7 days after campaign launch.
*   **Target Milestones:**
    *   **Day 14:** CTR stabilized above 5.0%, Quality Scores at 6-8 range.
    *   **Day 30:** Conversion rates above 3.0%, average CPA stabilized at $50.00.
    *   **Day 90:** Campaign ROAS exceeding 3.0x.
