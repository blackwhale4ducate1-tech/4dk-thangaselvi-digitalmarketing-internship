# Google Ads Bidding Strategy & Transition Plan

## 🎯 1. Purpose & Business Context
Bidding determines how much we pay for search clicks and how Google allocates our daily budget. For a new PPC account with no historical conversion data, jumping straight into automated "Smart Bidding" can cause Google's algorithm to bid erratically, leading to high CPCs and wasted budget.

This document details our **Bidding Strategy Progression**. We start with Manual CPC with Enhanced CPC (eCPC) to control keyword bid costs at launch, then transition to Target CPA (tCPA) or Maximize Conversions once the account has enough data.

---

## 📋 2. The Bidding Strategy Progression Plan

```text
  [PHASE 1: DAYS 1 - 30] ───────────────► [PHASE 2: DAY 30+]
  Manual CPC + eCPC                       Maximize Conversions / Target CPA
  (Build Data, Limit CPCs)                (Automated Bid Optimization)
```

### Phase 1: Manual CPC with Enhanced CPC (Launch Phase)
*   **Targeting Strategy:** Search campaigns (Brand, Competitor, Service).
*   **How it Works:** We manually set the maximum CPC bid for each keyword based on our research estimates (e.g. $1.50 for Brand, $3.20 for Service). Google is allowed to adjust these bids slightly using Enhanced CPC to optimize for conversions.
*   **Rationale:**
    *   Prevents Google from bidding $10+ on competitive keywords early on.
    *   Allows us to control bid adjustments for devices, hours, and geographic areas.
    *   Builds the baseline data needed for automated bidding.

### Transition Trigger (The 30/30 Rule)
Do not transition to automated Smart Bidding until the target campaign registers **at least 30 conversions within a rolling 30-day window** (45-50 conversions is preferred). Moving to automated bidding before this point can lead to poor performance due to lack of historical data.

### Phase 2: Maximize Conversions with Target CPA (Smart Bidding Phase)
*   **Targeting Strategy:** Service & Intent Search campaigns.
*   **Target CPA:** Set to **$50.00** (matches our business goals).
*   **How it Works:** Google's algorithm automatically adjusts bids at auction time using signals like user location, device, time of day, and search query to maximize leads within our Target CPA.
*   **Rationale:** Uses Google's machine learning to optimize bids for conversions rather than clicks.

---

## 🛠️ 3. Step-by-Step Transition Instructions

1.  **Monitor Conversion Volume:** Check your conversion column weekly to verify you have reached 30+ conversions in the last 30 days.
2.  **Verify Tag Health:** Go to **Tools and Settings > Measurement > Conversions** to confirm that conversion tracking is functioning correctly.
3.  **Adjust Campaign Settings:**
    *   Navigate to **Campaign Settings > Bidding**.
    *   Click **Change bid strategy**.
    *   Select **Maximize Conversions**.
    *   Check the box for "Set a target cost per action" and enter **$50.00**.
4.  **Monitor the Learning Phase:** Once transitioned, Google Ads will enter a **"Learning"** state for 7-14 days. Avoid making major bid or budget changes during this learning phase.

---

## 🖼️ 4. Example Screenshot Descriptions
*   **Screenshot 1: Google Ads Bidding Setup Window**
    *   *Description:* A screenshot of the Google Ads campaign settings panel. The Bidding strategy dropdown is open, displaying "Maximize Conversions" selected with a checkmark next to "Set a target cost per action (target CPA)" and "$50.00" entered in the input field.
*   **Screenshot 2: Bid Strategy Status Tracking**
    *   *Description:* The Campaign overview page showing the "Bid strategy type" column. The status box displays "Learning (Bid strategy active)" with a progress bar indicating days remaining in the learning phase.

---

## 🚫 5. Common Mistakes to Avoid
*   **Transitioning Too Early:** Moving to Target CPA with fewer than 15 conversions in the last 30 days. This causes the campaign to plateau and stop serving ads due to a lack of data.
*   **Setting the Target CPA Too Low:** Setting your Target CPA to $10.00 when your historical CPA is $50.00. This restricts Google's bidding algorithm, preventing your ads from winning auctions and stopping ad serving.
*   **Making Budget Changes During Learning:** Adjusting campaign budgets by more than 20% during the initial learning phase. This resets the algorithm's learning cycle, extending the learning phase.

---

## 📅 6. Expected Outcomes & Timelines
*   **Days 1-30 (Phase 1):** Maintain manual bid controls and build conversion history.
*   **Day 30 (Transition):** Assess conversion volumes and transition qualifying campaigns to Target CPA.
*   **Expected Results:** A stable Cost Per Lead (CPA) of **<$50.00** and a steady conversion volume by Month 2.
