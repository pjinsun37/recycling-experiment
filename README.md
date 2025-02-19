# Campus Recycling Experiment

# ‼️ Problem
Despite increasing awareness of sustainability, contamination in recycling bins remains a persistent challenge. Many individuals either fail to recycle correctly or do not recycle at all, leading to inefficiencies in waste management and undermining the effectiveness of recycling programs.

# 💡 Solution
**Could innovative recycling bin designs improve recycling accuracy?**

A team of NUS researchers conducted a controlled field experiment to evaluate whether simple design interventions — shaped bin openings and informational banners — could improve recycling behavior and reduce contamination rates.

The aim of this project was to analyze the given dataset and experimental design, applying econometric techniques to assess the intervention’s effectiveness.

# 🔬 Provided Experiment Design
The study was conducted in two locations on campus (ENGINE & UTOWN) and involved three sequential phases (each for 11-12 days):
- Phase 1 (Baseline): Standard recycling bins are used to measure initial recycling behavior.
- Phase 2 (Shaped Openings Introduced): Openings are modified to match recyclable item shapes (e.g., circular holes for cans, slots for paper).
- Phase 3 (Informational Banners Added): Banners with clear recycling instructions are placed on bins.

Since the dataset and experimental structure were pre-determined, our analysis focused on identifying causal effects within the existing study framework.

Second Phase (Shaped Openings)

<img width="570" alt="Screenshot 2025-02-19 at 3 34 30 PM" src="https://github.com/user-attachments/assets/b906c217-1089-4bee-9b91-7c81209a3899" />

<p>&nbsp;</p>

Third Phase (Informational Banners)

<img width="360" alt="Screenshot 2025-02-19 at 3 35 06 PM" src="https://github.com/user-attachments/assets/fde9b2af-3555-4715-8677-260783863ef5" />

<p>&nbsp;</p>

# 📊 Evaluation
To ensure causal inference, the study applied Difference-in-Differences (DiD) regression modeling to quantify treatment effects.

Key Steps:

**- Data Filtering:** The dataset includes 78 observations, with incomplete data points excluded to maintain consistency.

**- Parallel Trends Validation:** Pre-treatment trend analysis conducted to confirm methodological robustness.

  <img width="594" alt="Screenshot 2025-02-20 at 12 36 04 AM" src="https://github.com/user-attachments/assets/2d9bb998-af5b-4a09-9179-218595d3838c" />

  - Null Hypothesis: Trends in contamination rates between ENGINE and UTOWN are parallel during Phase 1 (b3 = 0)

**- DiD Regression Model:**

  <img width="867" alt="Screenshot 2025-02-20 at 12 34 21 AM" src="https://github.com/user-attachments/assets/bc1b4cee-18b5-4650-8e15-c4045060d7d3" />

  - Treatment = 1 if in the intervention group, 0 otherwise
  - Post = 1 if after intervention, 0 otherwise
  - Interaction terms (b3, b5) = Causal effect of interventions

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

<p>&nbsp;</p>

# 📂 Project Files

GP2Data: Contains datasets collected throughout the experiment.

regression_code.ipynb: Main notebook with code implementation of the Differences-in-Differences analysis.
