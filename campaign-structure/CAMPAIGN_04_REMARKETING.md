# Campaign 04: Remarketing Specification

## 🎯 1. Purpose & Business Context
Only 2% to 4% of visitors will convert on their first visit to a landing page. The remaining 96%+ leave without submitting a form or booking a call. Remarketing campaigns allow us to re-engage these past visitors and bring them back to complete their bookings.

This campaign targets custom audiences (past visitors and lead form dropouts) on the Google Display Network. It uses visual ads and client success testimonials to overcome objections and drive conversions at a lower cost.

---

## 📋 2. Campaign Configurations & Audience Lists

### A. Core Settings
*   **Daily Budget:** **$30.00/day** ($900/month).
*   **Bidding Strategy:** **Maximize Conversions**
    *   *Rationale:* Focuses on generating the maximum number of conversions from a highly targeted audience.
*   **Ad Formats:** Responsive Display Ads (RDAs) containing images, logos, headlines, and descriptions.
*   **Frequency Cap:** **5 impressions per user per day** (to prevent ad fatigue).

### B. Custom Audience Segments

#### Segment 1: Website Visitors (30 Days)
*   **Inclusion Rule:** Users who visited any marketing landing page or homepage in the last 30 days.
*   **Exclusion Rule:** Users who visited the `/thank-you` page (booked a call) or the `/client-portal` (active clients).

#### Segment 2: Lead Form Dropouts (60 Days)
*   **Inclusion Rule:** Users who visited the booking/calendar page `/book-call` but did not reach the confirmation page `/thank-you`.
*   **Exclusion Rule:** Exclude active clients and booked leads.

---

## 🛠️ 3. Step-by-Step Audience Setup & Launch Instructions

1.  **Set Up Audience Source:** Install the Google Ads Tag on your website (or link GA4 to Google Ads).
2.  **Create Audience Lists:**
    *   Go to **Tools and Settings > Shared Library > Audience Manager**.
    *   Click the blue **+** button and select **Website visitors**.
    *   Create `All Website Visitors - 30 Days` (URL contains `/`).
    *   Create `Booked Leads` (URL contains `/thank-you`).
    *   Create `Active Clients` (URL contains `/client-portal` or custom login URL).
3.  **Create Campaign:** Add a new campaign named `04_Display_Remarketing_US-UK-CA`. Set budget to $30.00/day.
4.  **Configure Targeting:**
    *   In the Ad Group, select **Audience segments**.
    *   Add `All Website Visitors - 30 Days` and `Lead Form Dropouts - 60 Days` as target segments.
    *   Add `Booked Leads` and `Active Clients` to the **Exclusion** list.
5.  **Set Frequency Cap:** Go to **Campaign Settings > Additional Settings > Frequency management**. Set a cap of 5 impressions per user per day.
6.  **Upload Ad Assets:** Upload brand logos, high-resolution fitness screenshots (coaches, client check-ins), and write ad copy focused on objections (e.g., "Ready for Real Results? Start Your 1-on-1 Coaching Journey").

---

## 🖼️ 4. Example Screenshot Descriptions
*   **Screenshot 1: Audience Segment Definition in Google Ads**
    *   *Description:* A screenshot of the Segment Builder in Google Ads Audience Manager. The page displays the rules: "Visitors of a page" URL contains `/` with membership duration set to "30 days" and an exclusion segment applied for "Booked Leads (URL contains `/thank-you`)".
*   **Screenshot 2: Frequency Capping Configuration Panel**
    *   *Description:* The Additional Settings panel in Google Ads displaying Frequency management options. The toggle is set to "Set limit" with a value of "5 impressions per day for this campaign".

---

## 🚫 5. Common Mistakes to Avoid
*   **Forgetting to Exclude Active Clients:** Showing ads to users who are already paying clients. This wastes budget and creates a poor user experience. Always exclude active client portals and conversion thank-you pages.
*   **No Frequency Capping:** Not setting a frequency cap. This results in users seeing your ads dozens of times a day, which can cause ad fatigue and lead to users blocking your ads.
*   **Targeting Small Audience Lists:** Launching a remarketing campaign when your audience list has fewer than 100 active users. Google Ads requires at least **100 active users** in a list to serve display ads.

---

## 📅 6. Expected Outcomes & Timelines
*   **Audience List Setup:** Complete audience setup on Day 1 (to start building lists early).
*   **Launch:** Launch campaign once the audience list reaches **1,000+ users** (typically within 2-3 weeks of launching search campaigns).
*   **Expected Results:** Achieve a low Cost Per Lead (CPA) of **<$40.00** and drive incremental conversions from users who previously left the site without converting.
