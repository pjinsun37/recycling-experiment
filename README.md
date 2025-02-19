# recycling-experiment

# 🔎 Problem
Despite increasing awareness of sustainability, contamination in recycling bins remains a persistent challenge. Many individuals either fail to recycle correctly or do not recycle at all, leading to inefficiencies in waste management and undermining the effectiveness of recycling programs.

# 💡 Solution
Could innovative recycling bin designs improve recycling accuracy?

A team of NUS researchers conducted a controlled field experiment to evaluate whether simple design interventions — shaped bin openings and informational banners — could improve recycling behavior and reduce contamination rates.

The aim of this project was to analyze the given dataset and experimental design, applying econometric techniques to assess the intervention’s effectiveness.

# 🔬 Provided Experiment Design
The study was conducted in two locations on campus (ENGINE & UTOWN) and involved three sequential phases:
- Phase 1 (Baseline): Standard recycling bins are used to measure initial recycling behavior.
- Phase 2 (Shaped Openings Introduced): Openings are modified to match recyclable item shapes (e.g., circular holes for cans, slots for paper).
- Phase 3 (Informational Banners Added): Banners with clear recycling instructions are placed on bins.

Since the dataset and experimental structure were pre-determined, our analysis focused on identifying causal effects within the existing study framework.

# 📊 Evaluation
To ensure causal inference, the study applied Difference-in-Differences (DiD) regression modeling to quantify treatment effects.

Key Steps:
- Parallel Trends Validation: Pre-treatment trend analysis conducted to confirm methodological robustness.
- Data Filtering: The dataset includes 78 observations, with incomplete data points excluded to maintain consistency.
- Comparability Adjustments: Observations across both locations were matched to control for baseline variations.

<p>&nbsp;</p>

Second Phase

<img width="570" alt="Screenshot 2025-02-19 at 3 34 30 PM" src="https://github.com/user-attachments/assets/b906c217-1089-4bee-9b91-7c81209a3899" />

<p>&nbsp;</p>

Third Phase

<img width="360" alt="Screenshot 2025-02-19 at 3 35 06 PM" src="https://github.com/user-attachments/assets/fde9b2af-3555-4715-8677-260783863ef5" />

<p>&nbsp;</p>

# 🔎 Key Findings

**✅ What Worked?**
- Shaped openings significantly reduced contamination rates for paper (↓ 2.5 pp) and can (↓ 15 pp).

**❌ What Didn’t Work?**
- Informational banners had no impact on paper or can recycling, and increased plastic contamination (↑ 9.1 pp) - likely due to confusing messaging.

<p>&nbsp;</p>

# 📢 Recommendations

- If immediate action is needed, consider gradually implementing shaped openings while re-evaluating messaging strategies for plastic recycling.
- **If time/budget allows, recommend conducting a redesigned experiment addressing observed limitations (below)**

<p>&nbsp;</p>

**⚠️ Limitations & Recommended Improvements**

- Uncontrolled External Factors: Events, campus schedules, and other influences may have affected behavior.
  - ✔️ Conduct surveys to track motivations & behaviors; use propensity score matching to adjust for external influences.
- Short Study Duration: Each phase lasted only 11–12 days, which may not reflect long-term behavioral changes.
  - ✔️ Increase intervention periods to evaluate long-term effects.
- Spillover Effects: The two study locations were only 15 minutes apart, potentially contaminating treatment groups.
  - ✔️ Use geographically separated test sites or track cross-location movement.
- Baseline Shift Between Phases: A one-month gap between Phases 2 and 3 may have introduced bias.
  - ✔️ Instead of relying on the original baseline, reset baselines before each intervention.
- Cumulative Treatment Effects: Since Phase 2 preceded Phase 3, it's unclear whether Phase 3 results were due to banners alone or a carryover effect from shaped openings.
  - ✔️ Randomize Treatment Order: Future studies should randomize intervention sequences to isolate individual effects and prevent cumulative bias.
