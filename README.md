# 🎯 Google Ads PPC Campaign Strategy & Playbook

<div align="center">

![Google Ads](https://img.shields.io/badge/Google_Ads-PPC-4285F4?style=for-the-badge&logo=google-ads&logoColor=white)
![Google Analytics 4](https://img.shields.io/badge/GA4-Analytics-orange?style=for-the-badge&logo=google-analytics&logoColor=white)
![Google Tag Manager](https://img.shields.io/badge/GTM-Tracking-2496ED?style=for-the-badge&logo=google-tag-manager&logoColor=white)
![Target CPA](https://img.shields.io/badge/Bidding-Smart_Bidding-34A853?style=for-the-badge&logo=google&logoColor=white)

**A comprehensive, production-grade Google Ads PPC Campaign Playbook for a high-ticket 1-on-1 Online Fitness Coaching business. Includes keyword lists, ad group copies, bidding transition schedules, landing page wireframes, and weekly performance reporting templates.**

[Overview](#1-campaign-overview) • [Structure](#3-campaign-architecture--hierarchy) • [Ad Copy](#5-responsive-search-ads-rsa-copywriting) • [Tracking](#6-conversion-tracking--gtm-integration) • [Reporting](#8-weekly-reporting-dashboard-template)

</div>

---

## 📋 Table of Contents

1. [Campaign Overview](#1-campaign-overview)
2. [Target Audience & Buyer Persona](#2-target-audience--buyer-persona)
3. [Campaign Architecture & Hierarchy](#3-campaign-architecture--hierarchy)
4. [Keyword Research & Matching Strategy](#4-keyword-research--matching-strategy)
5. [Responsive Search Ads (RSA) Copywriting](#5-responsive-search-ads-rsa-copywriting)
6. [Conversion Tracking & GTM Integration](#6-conversion-tracking--gtm-integration)
7. [Landing Page Wireframes & CRO Checklist](#7-landing-page-wireframes--cro-checklist)
8. [Weekly Reporting Dashboard Template](#8-weekly-reporting-dashboard-template)
9. [Bidding Strategy & Smart Bidding Roadmap](#9-bidding-strategy--smart-bidding-roadmap)
10. [RACI Matrix & Campaign Setup Workflows](#10-raci-matrix--campaign-setup-workflows)
11. [Ad Extensions Setup Guidelines](#11-ad-extensions-setup-guidelines)
12. [UTM Tagging & GA4 Parameter Configurations](#12-utm-tagging--ga4-parameter-configurations)
13. [Negative Keywords List](#13-negative-keywords-list)
14. [Competitor Copywriting Analysis](#14-competitor-copywriting-analysis)
15. [Verification Plan](#15-verification-plan)
16. [Project Changelog](#16-project-changelog)
17. [Contributing Guidelines](#17-contributing-guidelines)

---

## 1. Campaign Overview

This campaign playbook details the paid search acquisition framework designed for a premium **Online Fitness Coaching business**. The service is positioned as a high-ticket subscription offering, priced between **$150 and $300/month** (Customer Lifetime Value estimated at **$1,200** based on a 6-month average retention cycle). 

Paid acquisition is structured around **Google Search Ads** to capture active, high-intent searches. Rather than targeting general queries like "free home workouts," the campaign focuses on keywords like "personal trainer online for busy professionals," capturing leads actively looking to pay for a solution.

### Primary Objectives & Key Performance Indicators (KPIs)
- **Monthly Budget:** \$6,000 (\$200/day average split).
- **Target CPA (Cost per Acquisition / Lead):** < \$50 per booked Strategy Call.
- **Conversion Rate (Landing Page):** > 3.0% (Visitor to Strategy Call Lead).
- **Target ROAS (Return on Ad Spend):** 3.0x (Calculated against 3-month Customer Value).
- **Lead Quality Target:** > 75% qualified (income verification and commitment to coaching).

---

## 2. Target Audience & Buyer Persona

To keep ad spend focused and avoid waste, the campaign targets a specific buyer persona:

### Persona: "The Busy Professional" (Corporate Executive / Business Owner)
- **Demographics:** Age 30–55; Income > \$100k/year; Gender neutral.
- **Pain Points:** Long work hours, high stress, and limited time for meal prep or planning workouts. They struggle to find consistency with generic apps and value personalized guidance.
- **Motivation:** Desires a customized fitness and nutrition program that fits into a busy schedule, with 1-on-1 accountability.
- **Buying Objections:** "I don't have time," "I tried online coaching before and it didn't work," "It's too expensive."

### Target Settings Configuration
- **Locations:** United States & Canada.
- **Demographics:** Top 10% to 25% of household incomes.
- **Ad Schedule:** Monday to Friday, 6:00 AM to 9:00 PM (localized to searcher's time zone), matching when professionals are online.
- **Devices:** Optimized primarily for Mobile (estimated 70% of clicks) and Desktop (30%).

---

## 3. Campaign Architecture & Hierarchy

To maintain budget control and optimize ad delivery, the account uses a **4-Campaign Structure**:

```
                                  [ Google Ads Account ]
                                            │
         ┌──────────────────────┬───────────┴──────────┬──────────────────────┐
         ▼                      ▼                      ▼                      ▼
    01. Brand              02. Competitor         03. Service             04. Remarketing
  (Daily: $20)           (Daily: $40)           (Daily: $110)           (Daily: $30)
         │                      │                      │                      │
 ┌───────┴───────┐      ┌───────┴───────┐      ┌───────┴───────┐      ┌───────┴───────┐
 ▼               ▼      ▼               ▼      ▼               ▼      ▼               ▼
Brand Name    Founder  Competitor A  Competitor B Online Coach  Busy Pro   Visits  Email Leads
(Exact Match) (Phrase) (Phrase Match) (Phrase)  (Exact Match)  (Phrase)  (30 Days) (Remarket)
```

### Campaign Allocation Table

| Campaign ID | Campaign Name | Focus & Match Type | Daily Budget | Monthly Share | Bid Strategy |
|---|---|---|---|---|---|
| **PPC-01** | Brand Protection | Brand terms (Exact/Phrase) | \$20/day | 10% | Target Impression Share |
| **PPC-02** | Competitor Conquest | Competitor keywords (Phrase) | \$40/day | 20% | Maximize Clicks (Manual Cap) |
| **PPC-03** | Service & Intent | High-intent search terms (Exact/Phrase) | \$110/day | 55% | Maximize Conversions (Target CPA) |
| **PPC-04** | Audience Remarketing | Retargeting lists | \$30/day | 15% | Maximize Conversions |

---

## 4. Keyword Research & Matching Strategy

Our keyword list targets users showing clear buying intent. The list is structured into specific ad groups:

### Service Keywords List (`KEYWORDS.csv` mappings)

| Ad Group | Keyword | Match Type | Avg. CPC | Search Volume | Search Intent |
|---|---|---|---|---|---|
| **Online Coaching** | `online fitness coach` | Phrase | \$3.50 | 8,100/mo | Searching for online coaches |
| **Online Coaching** | `personal trainer online` | Exact | \$4.20 | 5,400/mo | Looking for personal trainers |
| **Busy Professionals**| `fitness coach for busy professionals` | Phrase | \$2.80 | 1,200/mo | Specific, high-value target query |
| **Busy Professionals**| `weight loss program corporate executives`| Exact | \$4.50 | 800/mo | High-ticket buyer persona query |
| **Custom Workouts** | `custom meal plan and workout online` | Phrase | \$3.10 | 2,400/mo | Looking for a custom solution |

### Negative Keywords List (`NEGATIVE_KEYWORDS.csv` mappings)

To prevent spending money on low-quality searches, the following negative keywords are configured at the account level:

```text
# Excluded search terms
"free", "cheap", "affordable", "discount", "jobs", "salary", "pdf download"
"youtube video", "reddit reviews", "app store", "at home workout no equipment"
"bodybuilding competition coach", "crossfit classes", "gym membership"
```

---

## 5. Responsive Search Ads (RSA) Copywriting

Our ads are structured using headlines and descriptions that address the busy professional's pain points while including clear call-to-actions (CTAs):

### Ad Group: Busy Professionals

#### Headlines (Max 30 characters)
1. `Online Fitness Coach for Pros` (Pin 1 - Focuses on the core offer)
2. `Get Fit in 3 Hours a Week` (Pin 2 - Solves the time constraint)
3. `Custom Workout & Diet Plans`
4. `Personal Trainer 1-on-1 Online`
5. `Made for Busy Executives`
6. `No Extreme Diets. Just Results.`
7. `Book Your Strategy Call` (Clear call-to-action)

#### Descriptions (Max 90 characters)
1. `1-on-1 online coaching tailored for busy executives. Get fit without spending hours in the gym.` (Pin 1)
2. `Custom meal plans, flexible workouts, and daily accountability. Book your free strategy call now.` (Pin 2)
3. `No cookie-cutter routines. We build custom fitness structures around your corporate schedule.`

---

## 6. Conversion Tracking & GTM Integration

Conversion tracking is set up using **Google Tag Manager** (GTM) to track Strategy Call bookings from the landing page.

### High-Level Event Flow

```
User Clicks Ad ──► Lands on Page with gclid ──► Clicks "Book Strategy Call"
  ──► Submits Calendly Widget ──► Calendly Event Triggered ──► GTM Listener
  ──► Send conversion event to Google Ads + GA4 (Purchase/Lead tag)
```

### Calendly GTM Custom HTML Script Listener

Add this listener in GTM to catch Calendly bookings and trigger conversion tags:

```html
<script>
window.addEventListener('message', function(e) {
  if (e.data.event && e.data.event.indexOf('calendly') === 0) {
    if (e.data.event === 'calendly.event_scheduled') {
      window.dataLayer = window.dataLayer || [];
      window.dataLayer.push({
        'event': 'calendly_booking_completed',
        'calendly_event_type': e.data.payload.event_type.uuid
      });
    }
  }
});
</script>
```

### Data Layer Structure

```json
{
  "event": "calendly_booking_completed",
  "calendly_event_type": "ev-busy-pro-strategy",
  "conversion_value": 150.00,
  "currency": "USD"
}
```

---

## 7. Landing Page Wireframes & CRO Checklist

Our landing page is optimized for conversions, ensuring that users arriving from search ads find a clear path to book a call:

### Landing Page Layout Blueprints

```text
┌────────────────────────────────────────────────────────┐
│ [Logo]                              [Call-to-Action]   │
├────────────────────────────────────────────────────────┤
│                                                        │
│  HEADLINE: Get Fit Without Giving Up Your Career       │
│  SUB-HEADLINE: 1-on-1 Fitness & Nutrition for Pros     │
│                                                        │
│  [Book Free Strategy Call Button]                      │
│                                                        │
│  [Hero Image: Fit professional in executive attire]    │
│                                                        │
├────────────────────────────────────────────────────────┤
│  SOCIAL PROOF: As Seen on Forbes, Bloomberg, etc.      │
├────────────────────────────────────────────────────────┤
│                                                        │
│  HOW IT WORKS:                                         │
│  1. Custom Assessment -> 2. Flexible Plan -> 3. Results│
│                                                        │
├────────────────────────────────────────────────────────┤
│  TESTIMONIALS: Before & After slider with details      │
├────────────────────────────────────────────────────────┤
│                                                        │
│  BOOKING ZONE: Inline Calendly scheduler widget        │
│                                                        │
└────────────────────────────────────────────────────────┘
```

### 20-Point Conversion Rate Optimization (CRO) Checklist
- [x] **Clear Above-the-Fold Value:** Headline explicitly mentions "Fitness for Professionals."
- [x] **Primary Call-to-Action:** High-contrast CTA button (e.g. "Book Strategy Call") placed top right and in the hero section.
- [x] **Fast Mobile Loading:** Page load times under **2.5 seconds** to prevent drop-offs.
- [x] **Social Proof:** Client transformation pictures and testimonials placed close to the booking form.
- [x] **Minimized Form Fields:** Intake questions limited to name, email, phone number, and goal select.
- [x] **Single-Topic Focus:** All navigation links removed to keep visitors focused on booking a call.

---

## 8. Weekly Reporting Dashboard Template

This report is delivered to the client every Monday morning, comparing performance metrics week-over-week (WoW):

```text
================================================================================
                    WEEKLY PPC PERFORMANCE DASHBOARD REPORT
================================================================================
Client: Online Fitness Coaching Co.
Reporting Period: May 24, 2026 - May 30, 2026
--------------------------------------------------------------------------------

1. EXECUTIVE SUMMARY METRICS
- Total Spend: $1,420.50 (Target: $1,400.00 | Variance: +1.4%)
- Impressions: 28,410
- Clicks: 1,562 (CTR: 5.50% | Target: >5.00%)
- Avg. CPC: $0.91 (Target: <$1.20 | Variance: -24.1%)
- Conversions (Strategy Calls Booked): 32 (Target: 28 | Variance: +14.2%)
- Conversion Rate: 2.05% (Target: >2.00%)
- Cost per Conversion (CPA): $44.39 (Target: <$50.00 | Variance: -11.2%)
- ROAS (On 3-Mo LTV): 3.38x (Target: >3.00x)

2. CAMPAIGN BREAKDOWNS
--------------------------------------------------------------------------------
Campaign Name        | Spend      | Clicks | Conversions | CPA      | ROAS
--------------------------------------------------------------------------------
01. Brand Protection | $145.00    | 320    | 8           | $18.12   | 8.27x
02. Competitor       | $285.50    | 242    | 3           | $95.16   | 1.57x
03. Service & Intent | $795.00    | 840    | 18          | $44.16   | 3.40x
04. Remarketing      | $195.00    | 160    | 3           | $65.00   | 2.30x
--------------------------------------------------------------------------------

3. TOP KEYWORDS BY CONVERSION PERFORMANCE
- "fitness coach online busy professionals" (Phrase) -> 12 Conversions | $38.50 CPA
- "personal trainer online corporate" (Exact) -> 8 Conversions | $42.00 CPA
- "[brand name coaching]" (Exact) -> 6 Conversions | $12.30 CPA

4. NEXT WEEK'S OPTIMIZATION PRIORITIES
- Action 1: Add negative keywords discovered from competitor search terms queries.
- Action 2: A/B test a new landing page headline targeting time efficiency.
- Action 3: Gradually raise the budget for the high-converting Service campaign.
================================================================================
```

---

## 9. Bidding Strategy & Smart Bidding Roadmap

The campaign uses a structured bidding plan, transitioning from manual control to Google's smart bidding algorithms over time:

```
                  ┌──────────────────────┐
                  │ Phase 1: Launch      │
                  │ Manual CPC bidding   │
                  └──────────┬───────────┘
                             │
                             │ Get 30+ conversions in 30 days
                             ▼
                  ┌──────────────────────┐
                  │ Phase 2: Growth      │
                  │ Maximize Conversions │
                  └──────────┬───────────┘
                             │
                             │ Stabilize booking numbers
                             ▼
                  ┌──────────────────────┐
                  │ Phase 3: Maturity    │
                  │ Target CPA bidding   │
                  └──────────────────────┘
```

### Bidding Stages Outline
- **Phase 1 (Launch - Days 1–30):** Use **Manual CPC Bidding** with Enhanced CPC enabled. This allows us to gather initial click data and find converting search terms while keeping budgets tight.
- **Phase 2 (Growth - Month 2):** Transition to **Maximize Conversions** once campaigns reach a baseline of 30+ conversions in 30 days, allowing Google's algorithms to maximize lead volume.
- **Phase 3 (Maturity - Month 3+):** Set a **Target CPA** once conversion rates stabilize. Set the cap at \$45 per lead to maintain a profitable lead cost.

---

## 10. RACI Matrix & Campaign Setup Workflows

To coordinate campaign launches, we use a **RACI Matrix** to define roles for each task:

| Task / Deliverable | PPC Specialist | Copywriter | Web Developer | Marketing Director |
|---|---|---|---|---|
| Keyword List | **Accountable/Responsible**| Consulted | Informed | Approved |
| Ad Copyblueprints | Consulted | **Responsible** | Informed | Accountable/Approved |
| Landing Page Dev | Informed | Consulted | **Responsible** | Accountable/Approved |
| GTM Tag Deployments | **Responsible** | Informed | Consulted | Accountable |
| Weekly Reports | **Accountable/Responsible**| Informed | Informed | Consulted |

---

## 11. Ad Extensions Setup Guidelines

Configure ad extensions to increase visibility and improve click-through rates (CTR):

- **Sitelink Extensions:**
  - Link 1: `Free Strategy Call` (Directs to the booking form scheduler).
  - Link 2: `Our Success Stories` (Links to before/after case studies).
  - Link 3: `1-on-1 Custom Pricing` (Links to pricing packages).
  - Link 4: `Meet the Coaches` (Links to coach profiles).
- **Callout Extensions:** Include key selling points: `24/7 Support`, `Custom Nutrition Plans`, `No Extreme Diets`, `Accountability Calls`.
- **Structured Snippets:** Highlight features: `Types: Custom Workouts, Diet Planning, Daily Text Support`.

---

## 12. UTM Tagging & GA4 Parameter Configurations

To track traffic source details accurately inside **Google Analytics 4 (GA4)** and CRM platforms, all campaign URLs must use our standard UTM structure:

```text
https://coach-fitness-pro.com/landing?utm_source=google&utm_medium=cpc&utm_campaign={campaignid}&utm_adgroup={adgroupid}&utm_term={keyword}
```

### Mapped Parameters Table

| Parameter | Assigned Value | Description |
|---|---|---|
| `utm_source` | `google` | Identifies search engines traffic |
| `utm_medium` | `cpc` | Identifies paid click actions |
| `utm_campaign` | `{campaignid}` | Dynamically inserts campaign IDs |
| `utm_adgroup` | `{adgroupid}` | Dynamically inserts ad group IDs |
| `utm_term` | `{keyword}` | Dynamically inserts searched keywords |

---

## 13. Negative Keywords List

A sample list from `research/NEGATIVE_KEYWORDS.csv` highlights terms we exclude to prevent paying for irrelevant clicks:

```csv
Keyword,Type,Exclusion Reason
free,Phrase,Avoid searches seeking free coaching services
cheap,Phrase,Exclude users looking for cheap workout apps
salary,Phrase,Exclude job seekers and salary research
bodybuilding,Phrase,Exclude contest prep training queries
crossfit,Phrase,Exclude users seeking local CrossFit gym classes
anytime fitness,Phrase,Exclude physical gym brand searches
weight loss pills,Exact,Exclude searches for weight loss supplements
```

---

## 14. Competitor Copywriting Analysis

We analyzed five major online fitness competitors to identify common messaging strategies and find angles to differentiate our copy:

- **Competitor A (High-volume apps):** Focuses on low cost and automated workouts.
  - *Differentiator:* We emphasize personal accountability and fully customized plans, matching busy professionals' expectations.
- **Competitor B (Local gym chains):** Focuses on physical locations.
  - *Differentiator:* We highlight the flexibility of online coaching, allowing professionals to work out on their own schedule.
- **Competitor C (Niche transformation coaches):** Focuses on extreme diets and high-intensity plans.
  - *Differentiator:* We position our coaching as a sustainable lifestyle change that fits into a busy corporate schedule.

---

## 15. Verification Plan

### Technical Ad Checks
1. Verify GTM tags fire correctly by running the GTM Preview tool and completing a test booking.
2. Confirm the Calendly listener captures scheduling events and pushes variables to the `dataLayer`.
3. Check UTM parameters in GA4 DebugView to verify source metrics are logged correctly.

### Landing Page Audits
1. Open the landing page on mobile and desktop viewports to check responsive scaling.
2. Run PageSpeed audits to verify mobile load times remain under **2.5 seconds**.

---

## 16. Project Changelog

### v1.0.0
- Launch of the initial project playbook.
- Account-level campaign structures and budget allocations.
- Responsive Search Ads (RSA) copywriting blueprints.
- Keyword and negative keyword spreadsheets setup.
- Google Tag Manager conversion tracking integration guide.

---

## 17. Contributing Guidelines

1. Proposed keyword additions must include average CPC metrics and search volume data.
2. Ad copy changes should be tested using A/B splits on landing pages before deploying account-wide.

---
#   4 d k - t h a n g a s e l v i - d i g i t a l m a r k e t i n g - i n t e r n s h i p