# Generative AI Usage Among Different Disciplines at UTM

This repository contains the data analysis, R code, and final report for a study investigating how generative AI usage and perception vary across different academic disciplines. The study was conducted at the University of Toronto Mississauga

## Project Overview
The emergence of generative AI has significantly impacted the educational landscape. This research aims to move beyond polarizing discourse by analyzing how a student's specific academic discipline influences their reliance on and perception of AI tools 

### Research Questions
**RQ1:** Does the perceived usefulness of generative AI for grasping course content differ across different disciplines?
**RQ2:** How does the proportion of assessments completed with the assistance of generative AI differ across academic disciplines?  
**RQ3:** Does the preference of using generative AI compared to traditional resources (TAs, professors, etc.) differ across academic disciplines? 

---

## Methodology
The study utilized **Simple Random Sampling (SRS)** to collect data from students in the STA304 course

**Population Size ($N$):** 200
**Sample Size ($n$):** 55 students
**Data Collection:** Conducted between October 7th and October 21st, 2024, using both physical questionnaires and Google Forms.
**Disciplines Analyzed:** Computer Science, Math, Economics, and "Other".

---

## Data Analysis & Statistical Tools
To address the non-normal distribution of the survey data, several robust statistical tests were employed using **R**:

**Mann-Whitney U Test (Wilcoxon Rank-Sum):** Used to compare means between [CS & Math] and [Economics & Other] groups for RQ1.
**Levene’s Test:** Performed to check for equality of variances across discipline groups.
**2-Sample Proportions Test:** Used for RQ2 and RQ3 to compare assignment completion rates and AI-preference ratios.
**ANOVA & Logistic Regression:** Utilized to explore broader relationships between discipline types and AI perceived usefulness.

---

## Key Findings
Across all three research questions, the study **failed to reject the null hypothesis** at a 95% confidence level.

**RQ1:** No significant difference was found in the perceived usefulness of AI for grasping course content between disciplines ($p = 0.3676$).
**RQ2:** The proportion of assessments completed with AI did not differ significantly between the grouped disciplines (Graded $p = 0.4$, Non-Graded $p = 0.88$).
**RQ3:** There was no statistically significant difference in the preference for AI over traditional resources ($p = 0.49$).

**Conclusion:** We do not have enough evidence to suggest that student perceptions and usage of generative AI vary significantly across these specific academic disciplines at UTM.

---

## Repository Structure
`GENAI_SURVEY.r`: The complete R script used for data cleaning, visualization (boxplots, stripcharts), and statistical testing.
`GENAI_Usage_Report.pdf`: The final formal report detailing the abstract, introduction, analysis, and limitations.
`Questionnarie (Responses) (2).xlsx`: The raw survey data (referenced in code).
