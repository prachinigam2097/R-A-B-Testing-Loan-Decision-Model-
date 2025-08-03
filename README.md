# A/B Testing Loan Decision Model – Advanced Data Analytics Project

## Problem Statement
A consumer lending company faced **high error rates in loan approvals** due to reliance on an outdated AI model. Loan officers were:
- **Approving bad loans** that defaulted (costing the company significant money).
- **Rejecting good loans** unnecessarily (losing profitable opportunities).

To address this, a **new AI model** was developed. Our team was tasked to **evaluate its impact** on decision quality through an **A/B test**:
- **Control group**: Loan officers used the old AI model.
- **Treatment group**: Loan officers used the new AI model.

The experiment’s goal was to determine if the **new model improved accuracy** in loan approvals, reduced financial risk, and influenced loan officers’ decision-making behaviour.

---

## Solution Approach
Our analysis focused on **data preparation, statistical testing, and business recommendations**:

### *Exploratory Data Analysis (EDA)**
- Identified **imbalances** between control and treatment groups and detected **data inconsistencies**.
- Analysed **loan officer performance** before and after AI guidance.

### *Defined Evaluation Metrics**
- **Profit Impact Error Index (PIEI):** A weighted metric combining Type I & II errors, factoring in profit per good loan and loss per bad loan.
- **AI Influence Index (AII):** Measured how much the AI model’s recommendations influenced loan officers’ final decisions.

### *Statistical Analysis**
- Conducted **Welch’s t-tests** to compare control vs. treatment on PIEI and AII.
- Calculated **Cohen’s d** effect sizes to assess the magnitude of improvement.

### *Key Findings**
- The **treatment group significantly outperformed control** on PIEI (p < 0.01), with a **large effect size**, showing the new AI model reduced costly errors.
- AII scores showed that the **new AI model increased loan officers’ alignment** with AI recommendations (p < 0.01), but further monitoring was advised to avoid over‑reliance.

### *Recommendations**
- **Rerun the experiment** with an improved design (intra‑office randomisation, cleaner data collection).
- **Incorporate financial metrics** (loan type, loan amount) for richer analysis.
- Proceed toward **phased adoption** of the new AI model once design flaws are resolved.

---

## Tech Stack
- **Languages:** R (tidyverse, ggplot2, effsize, pwr)
- **Techniques:** A/B testing, Welch’s t-test, Cohen’s d, power analysis
- **Data Sources:** Experimental loan officer decision data (10‑day trial)

---

## Impact
✔ Provided executives with **evidence-based recommendations** on whether to adopt the new AI model.  
✔ Introduced metrics (PIEI & AII) that improved how the company **measures financial risk & AI influence**.  
✔ Helped the analytics team **redesign the experiment** for more reliable, scalable future testing.

---

## Future Work
- Expand experiment with **larger sample size & randomisation improvements**.
- Add **dashboard visualisation** for PIEI & AII metrics.
- Explore integration with **real-time loan decision monitoring** systems.

---
