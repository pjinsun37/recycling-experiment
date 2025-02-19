# recycling-experiment

This project analyzes the impact of two recycling interventions on campus — shaped bin openings and informational banners — to assess their effectiveness in reducing contamination rates. Using Difference-in-Differences (DiD) analysis, we examine recycling behaviors across different locations to determine which interventions successfully improve waste sorting.

Second Phase

<img width="570" alt="Screenshot 2025-02-19 at 3 34 30 PM" src="https://github.com/user-attachments/assets/b906c217-1089-4bee-9b91-7c81209a3899" />


Third Phase

<img width="360" alt="Screenshot 2025-02-19 at 3 35 06 PM" src="https://github.com/user-attachments/assets/fde9b2af-3555-4715-8677-260783863ef5" />


**Key Findings**
- Shaped openings significantly reduced contamination rates for paper (-2.52pp) and cans (-15pp) but had no effect on plastic recycling.
- Informational banners had no impact on paper or can recycling and actually increased plastic contamination by 9.1pp, likely due to confusing signage.
- Recommendation: Shaped openings should be gradually implemented while re-evaluating messaging strategies for plastic recycling.

**Methodology**
- Study Design: Conducted in two phases across two locations on campus (ENGINE & UTOWN).
- Interventions Tested: Phase 2 (Shaped openings) / Phase 3 (Informational banners)
- Data Analysis: Applied Difference-in-Differences (DiD) regression modeling to measure the treatment effects.
- Parallel Trends Validation: Conducted pre-treatment trend analysis to ensure the robustness of the DiD methodology.

**Data & Adjustments**
- Dataset: Includes 78 observations after filtering out incomplete data points.
- Adjustments Made:
-   Excluded dates with missing values to maintain consistency.
-   Ensured matched observations across both locations to improve comparability.
