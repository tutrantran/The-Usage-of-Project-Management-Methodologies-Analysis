# 📊 Project Methodology Selection Under Uncertainty
### ART ANOVA • Multiple Regression • Monte Carlo Simulation

## Summary

Choosing between Waterfall, Agile, and Scrum is often based on preference or experience rather than evidence.  
This project applies **ART ANOVA, multiple regression, and Monte Carlo simulation** to evaluate methodology performance under realistic risk, cost, and schedule uncertainty.

Results show that while methodology appears important at first glance, **execution drivers (risk, budget overruns, schedule delays) explain most project success**.  
Among the three approaches, **Scrum delivers the strongest and most consistent outcomes**, offering the best risk–return profile.

---

## 1. Project Goals
This project answers three practical questions:
1. Which project management methodology leads to the highest success?
2. After controlling for risk, cost, and schedule, does methodology still matter?
3. Under uncertainty, which method has the lowest downside risk and most consistent performance?

## 2. Dataset Sources
- Synthetic Project Portfolio Dataset (1,000 projects)
- Designed using probability distributions to mimic realistic IT/software project environments.

Includes:
- Methodology (Waterfall / Agile / Scrum)
- Complexity level (High / Medium / Low)
- Risk, cost overrun, schedule delay
-Success rating, satisfaction, ROI

After preparation:
- 1,000 simulated projects
- Fully standardized & analysis-ready

## 3. Tech Stack
- R
- tidyverse (dplyr, ggplot2, tidyr)
- ARTool (ART ANOVA)
- MASS (Monte Carlo simulation)
- matrixcalc
- statistical modeling (regression, ANOVA, simulation)

## 4. Project Process
This project follows a simple, reproducible analytics workflow:

### 4.1. Business Understanding
- Define methodology comparison problem
- Clarify success–risk–performance hypotheses
- Identify decision criteria for project managers

### 4.2. Data Collection
- Synthetic portfolio dataset (1,000 projects)
- Probabilistic generation using realistic distributions

### 4.3. Data Cleaning & Preparation
- Factor encoding (Waterfall & High = baseline)
- Validate variable ranges
- Standardize project drivers
- Prepare modeling-ready dataset

### 4.4. Modeling & Analysis
- ART ANOVA (non-parametric)
- Multiple regression (incremental models)
- Driver impact analysis
- Monte Carlo simulation (10,000 scenarios/method)
- Sensitivity analysis (Spearman ρ)

### 4.5. Visualization & Insights
- Distribution plots
- ECDF comparisons
- Tornado sensitivity charts
- Risk–return profiles
- Business interpretation

### 4.6. Reporting
- Export tables & charts
- Generate summary KPIs
- Deliver actionable recommendations

## 5. Key Findings
### 5.1. Methodology Effect (ANOVA)
- Methodology significantly affects success
- Complexity has stronger impact
- No interaction effect

### 5.2. Regression (controlling for risk drivers)
- Model 1 → R² ≈ 44%
- Model 2 → R² ≈ 91%
- After adding risk/cost/schedule → methodology becomes statistically insignificant
👉 Execution quality matters more than methodology label

### 5.3. Monte Carlo Simulation
| Method    | Mean Success | P(>80)  | Downside Risk (<60) | Stability |
| --------- | ------------ | ------- | ------------------- | --------- |
| Waterfall | 76.2         | 36%     | 8.1%                | lowest    |
| Agile     | 79.4         | 48%     | 1.7%                | medium    |
| Scrum     | **81.0**     | **54%** | **0.5%**            | highest   |

🏆 Scrum shows the best risk–return profile

### 5.4. Sensitivity (Tornado)
Most impactful drivers:
- Risk exposure
- Budget overruns
- Schedule delays
- Methodology has smaller influence compared to these operational factors.

## 6. Skills Demonstrated
- Data wrangling & simulation design
- Non-parametric ANOVA (ART)
- Multiple regression modeling
- Monte Carlo risk analysis
- Sensitivity analysis
- Statistical storytelling
- Reproducible R workflows

## 7. Why This Matters
This analysis helps:
- Project Managers choose delivery methods based on data
- Quantify risk–return trade-offs
- Reduce failure probability
- Improve portfolio success rates
- Move from intuition → evidence-based decisions
- Turning analytics into smarter project strategy.
