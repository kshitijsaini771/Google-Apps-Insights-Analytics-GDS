# Google Play Store Market Intelligence Dashboard (Looker Studio)

## Problem Statement
The Android app ecosystem is highly competitive, and identifying **which categories, price models, and rating patterns drive success** is challenging without structured analytics. This project uses Looker Studio to transform **10,300 cleaned Google Play Store apps** into an interactive dashboard that supports **data-driven decisions** in app development, monetization, and marketing.

---

## Analysis Done
- Cleaned and standardized the original Kaggle dataset (`googleplaystore.csv`) for **10.3K apps**, removing duplicates, imputing missing values, and fixing data types [web:1].
- Processed installs, app size, price, categories, and dates in Python (`Google_Play_Store_Analytics_Cleaned_Data.ipynb`) to enable accurate filtering and aggregation.
- Defined **install tiers**: Very High (>1M), High (100K–1M), Medium (1K–100K), Low (<1K), and **rating bands**: Excellent, Very Good, Good, Fair, Poor.
- Key insights from the refined dataset:
  - **Average rating:** 4.2  
  - **Free apps:** 92.6% of total  
  - **Average installs per app:** 14.2M  
  - **Top categories by installs:** GAME (21.51%), COMMUNICATION (8.53%), SOCIAL (8.53).
- Built visual analyses:
  - **Rating vs Install Tier:** Very High install apps have stronger rating profiles (e.g., 35.75% Excellent vs 5.08% in Low tier).
  - **Trend over time (2010–2018):** Ratings and app quality improve notably in 2016–2018.
  - **Category performance:** GAME leads in both app volume and total installs, reinforcing it as a strategic focus area.
  - **Pricing insights:** Dominance of free apps highlights a freemium-driven ecosystem.

---

## Dashboard Overview
This Looker Studio dashboard provides an at-a-glance market view of the **Google Play Store**:

- **Scope:** ~9.6K cleaned apps, **146.6B installs**, average rating **4.2**, and **92.2% free apps**.
- **App & Reviews by Last Updated:** Line chart showing growth in updates and reviews from 2010–2018, capturing ecosystem maturity.
- **Top 10 Categories by App Count:** Treemap with FAMILY, GAME, TOOLS, and COMMUNICATION as leading segments.
- **Content Rating Distribution:** Donut chart where **80.9% of apps are rated “Everyone”**, and 11.1% target “Teen”, indicating broad family-friendly coverage.
- **Free vs Paid by Category:** Stacked bar chart highlighting that most categories are heavily skewed toward free apps.
- **Interactive Filters:** Category and Type (Free/Paid) filters support focused analysis by segment, monetization model, or niche.

<div align="center">

[Direct Link to Dashboard](https://lookerstudio.google.com/reporting/26f3c8eb-79d8-40f6-848b-b61473c93dd1)

</div>

![Looker Studio Dashboard](Looker.PNG)

---

## Recommendations
- **Double down on winning categories:** Prioritize GAME, FAMILY, TOOLS, and COMMUNICATION for new launches and feature investments.
- **Optimize freemium strategies:** With over 90% apps free, focus on in-app purchases, ads, and retention loops instead of upfront pricing.
- **Design for “Everyone”:** Given the dominance of “Everyone”-rated apps, build broadly accessible experiences while testing teen-focused niches where relevant.
- **Leverage high-install quality patterns:** Use insights from Very High tier apps (higher Excellent/Very Good share) as benchmarks for UX, performance, and update cadence.
- **Monitor recent cohorts:** Apps launched/updated between 2016–2018 show better ratings—adopt similar release and iteration patterns for future products.

---

**Author:** `Kshitij Saini`  
**LinkedIn:** [https://www.linkedin.com/in/kshitijsaini](https://www.linkedin.com/in/kshitijsaini-b950b7299?utm_source=share_via&utm_content=profile&utm_medium=member_android)
