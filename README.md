# GA4-E-Commerce-Audit-
A mid-size e-commerce brand is experiencing a common but costly problem: traffic is growing, but revenue isn't keeping pace. This audit investigates the full customer journey, from acquisition to purchase to identify where users drop off and where the biggest growth opportunities lie.
Note: This project uses Google's publicly available GA4 Demo Account
(Google Merchandise Store) to simulate a real client engagement.
# Objective
Answer five core business questions every e-commerce marketing team needs to know:

Where is traffic coming from — and is the channel mix healthy?

Who is the audience and how engaged are they?

Which content drives visits and which drives exits?

Where exactly do customers drop off before purchasing?

What should the brand prioritize to improve conversion?
# Tools & Stack
| Tool | Purpose |
|------|---------|
| **BigQuery (SQL)** | Querying raw GA4 event data |
| **Python (pandas, matplotlib)** | Data analysis & visualization |
| **Google Looker Studio** | Executive dashboard |
| **GitHub** | Portfolio & documentation |
# Key Findings
Critical — Conversion Funnel Drop-off
Out of 267,116 sessions, only 4,419 resulted in a purchase —
an overall conversion rate of just 1.6%. The most alarming drop
occurs at the very top: 77% of visitors never view a single product,
suggesting homepage engagement and navigation are the primary barriers.

| Funnel Stage | Users | Drop-off |
|---|---|---|
| Sessions | 267,116 | — |
| Viewed Item | 61,252 | -77% |
| Added to Cart | 12,545 | -80% |
| Began Checkout | 9,715 | -23% |
| Purchased | 4,419 | -55% |
#  Risk — Over-reliance on Organic Search
Organic Google drives 102,530 users — by far the dominant channel.
Direct traffic is second at 75,025. This heavy dependence on a single
channel creates significant business risk: any algorithm change could
severely impact revenue overnight.
# Insight — Unexpected Desktop Dominance
57.9% of users visit via desktop, which is unusual for modern
e-commerce where mobile typically dominates. This suggests an older
or more professional audience — and signals that the mobile experience
may be underinvested relative to where the industry is heading.
# Opportunity — Untapped International Markets
The US drives 118,493 users while India (25,367), Canada (20,268),
and UK (8,527) show meaningful but underdeveloped traffic. There is clear
potential for localized campaigns targeting English-speaking markets.
# Trend — Seasonal Peak in December
Monthly user data shows a clear peak in December 2020 (holiday season),
followed by a January dip. The brand is not capitalizing on pre-holiday
traffic building in October–November, missing warm-up conversion opportunities
# Recommendations
1. Fix the homepage → product discovery gap (highest priority)
77% of visitors leave without viewing a product. Improve homepage
personalization, add featured product sections, and A/B test navigation
structure to reduce this drop.
2. Diversify traffic sources
Invest in paid social and email marketing to reduce dependency on organic
search. A single-channel strategy is a business continuity risk.
3. Optimize mobile experience
Despite desktop dominance today, mobile is the direction of travel.
Audit mobile UX — page speed, checkout flow, and product imagery —
before this becomes a competitive disadvantage.
4. Build a pre-holiday campaign calendar
Start driving traffic and building remarketing lists in October for
December conversion. The data shows strong December intent — capture
it earlier in the funnel.
5. Test international paid campaigns
India and Canada show organic interest with zero paid investment.
Low-cost test campaigns in these markets could yield strong ROAS
given the existing organic baseline.
# Dashboard
🔗 View Live Looker Studio Dashboard
The dashboard includes 5 pages:

Summary & Trends
Device & Geographic Breakdown
Traffic Source Analysis
Conversions & Top Pages
eCommerce Performance
# The full Python analysis
The full Python analysis is available in /notebook/GA4_E-Commerce_Audit.ipynb
It covers data extraction via BigQuery API, cleaning, analysis,
and visualization — structured as a narrative from business question
to actionable insight.
#SQL Queries
All BigQuery SQL queries are available in the /sql folder:

traffic_overview.sql — Monthly sessions and user trends

traffic_sources.sql — Channel and source breakdown

device_breakdown.sql — Device category analysis

country_breakdown.sql — Geographic user distribution

conversion_funnel.sql — Full funnel from session to purchase
# Methodology
Raw GA4 event-level data was queried directly from Google's public
BigQuery dataset (bigquery-public-data.ga4_obfuscated_sample_ecommerce).
Data was pulled into Python via the BigQuery API, cleaned using pandas,
and visualized using matplotlib. The Looker Studio dashboard connects
directly to the GA4 Demo Account property for live, interactive reporting.
# About
This project was created as part of a marketing analytics portfolio
demonstrating end-to-end analysis capability — from raw data extraction
to executive-level insight delivery.
Skills demonstrated: SQL · Python · GA4 · BigQuery · Looker Studio ·
Data Storytelling · Marketing Analytics · Conversion Optimization

