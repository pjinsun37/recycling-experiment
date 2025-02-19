# recycling-experiment

This project analyzes the impact of two recycling interventions on campus — shaped bin openings and informational banners — to assess their effectiveness in reducing contamination rates. Using Difference-in-Differences (DiD) analysis, we examine recycling behaviors across different locations to determine which interventions successfully improve waste sorting.

**Key Findings**
- Shaped openings significantly reduced contamination rates for paper (-2.52pp) and cans (-15pp) but had no effect on plastic recycling.
- Informational banners had no impact on paper or can recycling and actually increased plastic contamination by 9.1pp, likely due to confusing signage.
- Recommendation: Shaped openings should be gradually implemented in high-traffic areas (e.g., malls, office complexes, tourist attractions) while re-evaluating messaging strategies for plastic recycling.

**Methodology**
- Study Design: Conducted in two phases across two locations (ENGINE & UTOWN).
- Interventions Tested:
-   Phase 2: Shaped openings
-   Phase 3: Informational banners
- Data Analysis: Applied Difference-in-Differences (DiD) regression modeling to measure the treatment effects.
- Parallel Trends Validation: Conducted pre-treatment trend analysis to ensure the robustness of the DiD methodology.

**Data & Adjustments**
- Dataset: Includes 78 observations after filtering out incomplete data points.
- Adjustments Made:
-   Excluded dates with missing values to maintain consistency.
-   Ensured matched observations across both locations to improve comparability.
