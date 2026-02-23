# Comparative Analysis of Single-Activity Income Strategies in Stardew Valley

This repository contains the full implementation, dataset, visualizations, and final paper for a quantitative study analyzing income optimization strategies in **Stardew Valley**.

The project empirically compares four exclusive income-generating activities — **Farming, Fishing, Mining, and Foraging** — across one full in-game year (112 days per activity) under controlled time and energy constraints.

📄 Full paper included: `CCDATSCL__FinalPaper.pdf`

---

## 📌 Research Objective

The study investigates:

> Which single income-generating activity yields the highest profitability and time-based efficiency when played exclusively for one in-game year?

Performance was evaluated using:

- **Net Activity Income** (Primary Activity Gold − Expenses)
- **Gold Per Minute (GPM)** (Net Activity Income ÷ Time Spent)

The experiment isolates each activity to remove multitasking effects and measure its independent economic potential.

---

## 🧪 Experimental Design

- Single-subject, controlled design
- 4 full in-game years (one per activity)
- 448 total daily observations (112 per activity)
- Manual logging of financial, environmental, and progression variables
- Statistical comparison of income distributions

### Activities Tested

- 🌾 Farming
- 🎣 Fishing
- ⛏ Mining
- 🌿 Foraging

---

## 📊 Dataset Overview

Final dataset:
- **448 observations**
- **26 variables**
- Temporal, environmental, financial, and progression features

### Key Derived Variables

- `Net Activity Income`
- `Gold Per Minute`
- `Continuous Game Day`
- Skill and tool progression encodings

Data cleaning included:
- Time conversion to minutes
- Categorical encoding
- Feature engineering
- Ordered progression tiers
- Removal of non-contributory columns

---

## 📈 Statistical Analysis

Because income distributions were non-normal:

- **Shapiro–Wilk Test** → confirmed non-normality
- **Kruskal–Wallis H Test** → detected significant differences across activities
- **Dunn’s Post-Hoc Test (Bonferroni corrected)** → identified pairwise differences

Significance level: α = 0.05

Results confirmed statistically significant differences in both:
- Net Activity Income
- Gold Per Minute (GPM)

---

## 🔎 Key Findings

### 🥇 Fishing – Highest Mean & Cumulative Income

- Highest **mean daily net income**: 923.72g
- Highest cumulative net income over one year
- Low expense burden
- Stable, low-volatility returns
- Best for risk-averse strategy

### ⚡ Farming – Highest Median Income & Time Efficiency

- Highest **median daily net income**: 1,387.50g
- Highest **median GPM**: 8.46
- Highest cumulative gross earnings (>180,000g)
- High volatility due to crop cycle
- Best for high-efficiency, high-variance strategy

### ⛏ Mining – Moderate, Luck-Sensitive Returns

- Episodic income spikes
- Strong dependence on daily luck
- Moderate efficiency
- Middle-ground strategy

### 🌿 Foraging – Lowest Profitability & Efficiency

- Lowest mean and median income
- Lowest GPM
- Highest average time spent per day
- Zero expenses but low scalability
- Best used as a supplementary activity

---

## 📊 Trade-Off Summary

| Activity   | Stability | Peak Income | Efficiency | Volatility |
|------------|----------|------------|------------|------------|
| Fishing    | High     | Moderate   | Moderate   | Low        |
| Farming    | Moderate | Very High  | Very High  | High       |
| Mining     | Moderate | Moderate   | Moderate   | Medium     |
| Foraging   | High     | Low        | Low        | Low        |

No activity dominates across all metrics.

Optimal choice depends on:
- Risk tolerance
- Capital availability
- Time efficiency preference
- Long-term vs short-term goals

---

## 🛠 Tools & Technologies

- Python
- pandas
- numpy
- matplotlib
- seaborn
- scipy
- scikit-posthocs

---

## ⚠ Limitations

- Single-subject design
- One-year activity isolation
- Manual data logging
- No access to post-Year-1 unlocks
- Main island only (no island expansion testing)

Results reflect distributional comparisons within this controlled experiment rather than universal gameplay optimization.

---

## 🔬 Future Work

- Multi-year simulations
- Automated data collection via mods/scripts
- Mixed-activity strategy modeling
- Stamina tracking
- Multi-island comparison
- Seasonal replication studies

---

## 🎓 Academic Context

This research contributes to:

- Virtual economy modeling
- Resource allocation under constraints
- Optimization in simulated systems
- Risk vs reward trade-off analysis

The study demonstrates how structured game systems function as controlled economic environments for empirical analysis.

---

## 🎮 Conclusion

Under exclusive one-year conditions:

- **Fishing maximizes cumulative stability**
- **Farming maximizes time efficiency and peak-day returns**
- **Mining offers moderate stochastic gains**
- **Foraging is economically limited as a standalone strategy**

The findings reinforce that optimal strategy selection depends on player objectives and tolerance for volatility rather than a single universally dominant activity.
