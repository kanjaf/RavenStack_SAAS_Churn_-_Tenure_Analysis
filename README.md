Executive Summary This project analyzes user behavior across 5,000+ accounts to identify the primary drivers of churn and the characteristics of "Power Users." By bridging feature-level event data with account-level outcomes, I isolated a "Safety Zone" of 400+ days tenure and audited the impact of experimental (Beta) features on long-term retention.

The "Churn Gap" & Tenure Analysis Using a custom-engineered tenure calculation, I identified a significant "Value Gap" in the first 250 days.
Average Churned Tenure: ~250 days.

The "Safety Zone": Users who reach 400 days of tenure exhibit nearly 0% churn probability, becoming "sticky" long-term assets.

Infant Mortality: A subset of users churns within just 3 days, indicating critical friction in the initial onboarding experience.

Usage Intensity & "The Peak" I analyzed total feature usage density to find the "active user" threshold.
The Usage Peak: Most users (both churned and active) engage with approximately 45 feature events.

Retention Signal: High-frequency usage (125+ events) is almost exclusively found in the active cohort, suggesting that depth of usage is a leading indicator of health.

Friction & Beta Feature Audit I conducted a diagnostic audit of experimental features and technical errors.
The Frustration Index: Active users in the primary usage peak (25-60 uses) experience an average of 1.0 technical error per session.

Beta Impact: Users engaging with Beta features showed a slightly higher churn rate (23.7%) compared to standard users (22.1%).

Strategic Recommendation: While Beta features drive engagement, the 1.6% churn increase suggests a need for improved stability or better "Time-to-First-Value" in the experimental roadmap.

Technical Stack Python (Pandas/NumPy): For relational data joining and behavioral cohorting.
Seaborn/Matplotlib: For KDE distribution plots and friction heatmaps.

Data Architecture: Managed a five-table schema including accounts, feature events, and support tickets.

Key Recommendations Bridge the 100-Day Gap: Implement a re-engagement campaign for users approaching the 100-day mark to push them toward the 400-day "Safety Zone".
Onboarding Audit: Focus engineering efforts on reducing errors for users in their first 25 usage events to mitigate "Infant Mortality" churn.

Beta Stability: Prioritize bug fixes for Beta features, as they currently represent a minor churn risk for high-intensity users.
