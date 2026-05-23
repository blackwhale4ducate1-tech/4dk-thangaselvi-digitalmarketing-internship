# Online Fitness Coaching Google Ads PPC Campaign Strategy & Playbook

Welcome to the **Online Fitness Coaching Google Ads PPC Campaign Strategy Repository**. This repository contains a structured, end-to-end framework for launching, managing, and optimizing paid search campaigns to acquire high-ticket 1-on-1 online fitness coaching clients. 

This plan is tailored for a subscription-based coaching business model priced at **$150 to $300/month** (Customer Lifetime Value: ~$1,200), focusing on busy professionals who value customized training programs and nutrition guides.

---

## 📖 Table of Contents
1. [Purpose & Business Goals](#-purpose--business-goals)
2. [Campaign Overview & Budget Allocation](#-campaign-overview--budget-allocation)
3. [Target PPC Metrics (KPIs)](#-target-ppc-metrics-kpis)
4. [Repository Directory Structure](#-repository-directory-structure)
5. [Team Ownership Matrix (RACI)](#-team-ownership-matrix-raci)
6. [Campaign Setup & How to Deploy](#-campaign-setup--how-to-deploy)
7. [Common Execution Mistakes to Avoid](#-common-execution-mistakes-to-avoid)
8. [Expected Outcomes & Optimization Timeline](#-expected-outcomes--optimization-timeline)

---

## 🎯 Purpose & Business Goals

The goal of this PPC program is to acquire clients for our **1-on-1 Online Fitness Coaching program**.
*   **Target Audience:** Busy professionals (ages 25-50) struggling with weight loss, strength training, or diet planning who are willing to pay a premium for personalized accountability.
*   **Core Offer:** 1-on-1 customized workout routine, macro-based nutrition coaching, weekly video check-ins, and direct access to a dedicated coach.
*   **Funnel Path:** Google Search Ad $\rightarrow$ Ad Group Specific Landing Page $\rightarrow$ Lead Form submission (free strategy call) $\rightarrow$ Close on phone call.

---

## 💰 Campaign Overview & Budget Allocation

Our monthly budget is set at **$6,000/month ($200/day)**. We distribute the budget across four core campaigns to balance brand protection, high-intent service searches, competitor targeting, and audience retargeting:

| Campaign Name | Focus & Targeting Type | Daily Budget | Monthly Budget | Budget % |
| :--- | :--- | :---: | :---: | :---: |
| **01. Brand Protection** | Brand terms (e.g., "FitLife Coaching") | $20/day | $600/month | 10% |
| **02. Competitor Conquest** | Target competitor brands (e.g., "CoPilot", "Future Fit") | $40/day | $1,200/month | 20% |
| **03. Service & Intent** | High-intent terms (e.g., "hire online fitness coach") | $110/day | $3,300/month | 55% |
| **04. Remarketing** | Past website visitors & lead form dropouts | $30/day | $900/month | 15% |

---

## 📈 Target PPC Metrics (KPIs)

*   **Target ROAS (Return on Ad Spend):** **3.0x** (calculated on a 3-month Customer Value baseline).
*   **Target CPA (Cost Per Acquisition / Lead):** **$50.00** per booking strategy call.
*   **Target Customer CAC (Customer Acquisition Cost):** **$150.00** (assuming a 33% close rate from call to client).
*   **Click-Through Rate (CTR):** **>5.0%** (search campaign average).
*   **Quality Score Target:** **>7/10** across all core service keywords.

---

## 📂 Repository Directory Structure

The repository files are organized logically to guide you from keyword research to campaign setup and weekly reporting:

```text
/google-ads-ppc-fitness
│
├── README.md                           # Campaign overview, budget, targets, and setup (This file)
│
├── /research
│   ├── KEYWORD_RESEARCH.md             # Keyword methodology, search volume, and CPC analysis
│   ├── KEYWORDS.csv                    # Database of 30+ fitness keywords mapped to ad groups
│   ├── NEGATIVE_KEYWORDS.csv          # List of keywords to exclude (free, cheap, jobs, etc.)
│   └── COMPETITOR_ADS.md               # 5 competitor ads analyzed for hooks and positioning gaps
│
├── /campaign-structure
│   ├── CAMPAIGN_STRUCTURE.md           # Account structure: Campaigns, Ad Groups, and Settings
│   ├── CAMPAIGN_01_BRAND.md            # Brand protection campaign specifications
│   ├── CAMPAIGN_02_COMPETITOR.md       # Competitor conquest campaign specifications
│   ├── CAMPAIGN_03_SERVICE.md          # Core fitness coaching service campaign details
│   └── CAMPAIGN_04_REMARKETING.md      # Custom audience remarketing specifications
│
├── /ad-copy
│   ├── AD_GROUP_01.md                  # Brand Responsive Search Ads (RSAs) and pinning strategy
│   ├── AD_GROUP_02.md                  # Competitor Responsive Search Ads (RSAs)
│   ├── AD_GROUP_03.md                  # Service/Intent Responsive Search Ads (RSAs)
│   └── COPY_BEST_PRACTICES.md          # Fitness copywriting tips, hooks, and DKI formatting
│
├── /extensions
│   └── AD_EXTENSIONS.md                # Copy for Sitelinks, Callouts, Snippets, and Lead Forms
│
├── /landing-pages
│   ├── LANDING_PAGE_BRIEF.md           # Visual & copy layout briefs for each ad group
│   └── CRO_CHECKLIST.md                # 20-point conversion rate optimization checklist
│
├── /bidding
│   └── BIDDING_STRATEGY.md             # Bid strategy selection and manual-to-automated plan
│
├── /tracking
│   ├── CONVERSION_TRACKING.md          # Google Tag Manager triggers, tags, and data layers
│   └── UTM_PARAMETER_GUIDE.md          # UTM naming conventions for tracking in CRM/GA4
│
└── /reporting
    ├── KPI_TARGETS.md                  # Target metrics, definitions, and performance benchmarks
    └── WEEKLY_REPORT_TEMPLATE.md       # Standardized table and logs for weekly client reporting
```

---

## 👥 Team Ownership Matrix (RACI)

Clear roles ensure campaigns are launched on time and budget pacing is monitored daily.

| Deliverable / Task | PPC Specialist | Content Writer | Landing Page Dev | Fitness Lead / Director |
| :--- | :---: | :---: | :---: | :---: |
| **Keyword Research & Negatives**| **A** / **R** | **I** | **I** | **C** |
| **Ad Copywriting & Pinned Ads** | **C** | **R** | **I** | **A** |
| **Landing Page Briefs & CRO**   | **R** | **R** | **R** / **A** | **C** |
| **Bidding & Budget Pacing**     | **A** / **R** | **I** | **I** | **I** |
| **Conversion Tag Implement**    | **R** | **I** | **A** / **R** | **I** |
| **Weekly KPI Reporting**        | **A** / **R** | **I** | **I** | **C** |

---

## ⚙️ Campaign Setup & How to Deploy

### Step 1: Initialize Your Google Ads Account
1.  Set up a new Google Ads account or create a sub-account within your Manager Account (MCC).
2.  Set billing settings to match your **$6,000/month** budget.

### Step 2: Upload Negative Keyword Lists
1.  Navigate to **Tools and Settings > Shared Library > Negative Keyword Lists**.
2.  Create a list named `Global Negatives` and upload all keywords from [NEGATIVE_KEYWORDS.csv](file:///d:/4DK/Projects/Marketting/google-ads-ppc-fitness/research/NEGATIVE_KEYWORDS.csv).
3.  Apply this negative list to all active search campaigns.

### Step 3: Implement Tracking
Deploy tracking codes using the instructions in [CONVERSION_TRACKING.md](file:///d:/4DK/Projects/Marketting/google-ads-ppc-fitness/tracking/CONVERSION_TRACKING.md) to ensure conversions map to the right keywords.

### Step 4: Build Landing Pages
Pass the landing page guidelines in [LANDING_PAGE_BRIEF.md](file:///d:/4DK/Projects/Marketting/google-ads-ppc-fitness/landing-pages/LANDING_PAGE_BRIEF.md) to your designers/developers. Ensure pages pass all points in [CRO_CHECKLIST.md](file:///d:/4DK/Projects/Marketting/google-ads-ppc-fitness/landing-pages/CRO_CHECKLIST.md).

### Step 5: Upload Campaigns, Keywords, and Ad Copy
1.  Import campaigns using Google Ads Editor or the online interface.
2.  Input keywords from [KEYWORDS.csv](file:///d:/4DK/Projects/Marketting/google-ads-ppc-fitness/research/KEYWORDS.csv) into respective campaigns.
3.  Copy and paste the responsive search ads and descriptions from the `/ad-copy` folder.
4.  Configure sitelink, callout, and lead form extensions as specified in [AD_EXTENSIONS.md](file:///d:/4DK/Projects/Marketting/google-ads-ppc-fitness/extensions/AD_EXTENSIONS.md).

---

## 🚫 Common Execution Mistakes to Avoid

1.  **Using All Broad Match Keywords:** Launching with pure broad match keywords without a negative list. This wastes budget on irrelevant searches like "free workouts at home". Stick to phrase and exact matches initially.
2.  **Driving Traffic to the Homepage:** Directing users searching for "custom diet coach" to your homepage instead of a specific landing page. This leads to high bounce rates and low conversion rates.
3.  **Bypassing Brand Campaign Setup:** Ignoring brand keywords because "we already rank organically". Competitors will bid on your brand name and capture high-intent leads if you do not protect your brand space.
4.  **No Weekly Budget Cap Check:** Forgetting to set strict campaign daily caps, allowing Google to spend up to 2x the daily budget in a single day during search volume spikes.

---

## 📅 Expected Outcomes & Optimization Timeline

*   **Days 1 - 3 (Setup):** Landing pages deployed, GTM conversion tags tested, campaigns uploaded in paused state.
*   **Day 4 (Launch):** Launch search campaigns with Manual CPC bidding to control keyword click prices.
*   **Weeks 1 - 2 (Pacing):** Monitor search terms daily, add new negative keywords, and adjust keyword bids to maintain average ad position 1-3.
*   **Weeks 3 - 4 (Optimization):** Analyze ad copy performance, pause low-performing headlines/descriptions, and compile the first weekly reports.
*   **Day 30+ (Smart Bidding):** Once we reach 30+ conversions in a campaign, transition from Manual CPC to Target CPA or Maximize Conversions bidding.
*   *Expected Outcomes:* Lead cost (CPA) stabilized at **<$50/lead**, Conversion Rate **>3%**, and ROAS exceeding **3.0x** by Month 3.
#   4 d k - t h a n g a s e l v i - d i g i t a l m a r k e t i n g - i n t e r n s h i p  
 