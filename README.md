# recycling-experiment

This project analyzes the impact of two recycling interventions conducted by campus researchers — shaped bin openings and informational banners — to assess their effectiveness in reducing contamination rates. Using Difference-in-Differences (DiD) analysis, we examine recycling behaviors across different locations to determine which interventions successfully improve waste sorting.

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

<p>&nbsp;</p>

Second Phase

<img width="570" alt="Screenshot 2025-02-19 at 3 34 30 PM" src="https://github.com/user-attachments/assets/b906c217-1089-4bee-9b91-7c81209a3899" />

<p>&nbsp;</p>

Third Phase

<img width="360" alt="Screenshot 2025-02-19 at 3 35 06 PM" src="https://github.com/user-attachments/assets/fde9b2af-3555-4715-8677-260783863ef5" />

<p>&nbsp;</p>

**Key Findings**
- Shaped openings significantly reduced contamination rates for paper (-2.52pp) and cans (-15pp) but had no effect on plastic recycling.
- Informational banners had no impact on paper or can recycling and actually increased plastic contamination by 9.1pp, likely due to confusing signage.
- Recommendation: Refer to limitations to conduct re-designed experinment. If time / budget does not allow, consider gradually implementing shaped openings while re-evaluating messaging strategies for plastic recycling.

**Key Limitations**
- Unobserved External Factors: External influences such as campus events and academic schedules may have affected recycling behavior. These were not controlled for in the study.
- Short Study Duration: Each phase lasted only 11–12 days, which may not be enough time for long-term behavioral adjustments.
- Potential Spillover Effects: The two study locations (ENGINE & UTOWN) were only 15 minutes apart, increasing the risk of behavioral contamination across groups.
- Baseline Shift Between Phases: A one-month gap between Phase 2 (shaped openings) and Phase 3 (informational banners) may have introduced bias, making it harder to assess the true effect of banners.
- Cumulative Treatment Effects: Since Phase 2 preceded Phase 3, it is unclear whether Phase 3 results were due to banners alone or carryover effects from shaped openings.

**Points of Imporvement**
- Control for External Factors: Conduct surveys to track motivations and behaviors, and use statistical controls (e.g., propensity score matching) to account for external influences.
- Increase Study Duration: Extending intervention periods would help assess long-term effects and behavioral sustainability.
- Reduce Spillover Effects: Future experiments should be conducted in geographically separated locations or include tracking mechanisms for cross-location movement.
- Establish New Baselines for Each Phase: Instead of using the original baseline, setting a new baseline before each phase would better account for behavioral shifts.
- Randomize Treatment Order: Future experiments should randomize intervention sequences to separate individual effects and reduce cumulative treatment bias.
