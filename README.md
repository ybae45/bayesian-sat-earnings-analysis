## Project Intro/Objective
The purpose of this project is to examine the relationship between average SAT scores at U.S. universities and post-graduation earnings, and to understand whether this relationship varies across geographic regions. While standardized test scores are often used as a proxy for college selectivity and student aptitude, their role in predicting long-term economic outcomes remains debated.

This project aims to provide a data-driven and probabilistic analysis of this relationship using Bayesian hierarchical modeling, allowing for uncertainty quantification and regional heterogeneity. By leveraging large-scale institutional data, this study contributes to the broader discussion on education outcomes and income inequality.

Specifically, this project includes:

Descriptive statistics and exploratory data analysis (EDA) to understand the distributions and relationships between SAT scores and earnings

Data cleaning and preprocessing to ensure consistency and comparability across institutions and years

A Bayesian hierarchical regression framework to model earnings while accounting for regional variation

## Preliminary Literature Review
- https://www.researchgate.net/publication/383720798_A_Case_Study_of_the_Correlation_Between_SAT_Scores_and_Future_Incomes
  -   Summary: This paper conducts a correlation analysis using a questionnaire method and Pearson’s coefficient, in addition to exploring the relationship between SAT scores and position level of post grad jobs. Results show a significant positive correlation between SAT scores and future incomes. The Pearson correlation coefficient of SAT scores for the obtained samples is 0.355 and the significance is <0.01, which is statistically significant.
- https://academic.oup.com/qje/article/135/3/1567/5741707
- https://www.travistang.com/blog/higher-spending-leads-to-poorer-education-a-bayesian-statistics-project-using-monte-carlo-techniques/
- https://pmc.ncbi.nlm.nih.gov/articles/PMC9036241/

## Project Description
We used College Scorecard data, institution-level data files for 1996-97 through 2022-23 containing aggregate data for each institution. Data inclues information on institutional characteristics, enrollment, student aid, costs, and student outcomes.
This project uses U.S. Department of Education College Scorecard institution-level data from academic years 1996–1997 through 2022–2023. The dataset contains aggregated information for each institution, including:

- Average SAT scores
- Median earnings of graduates (measured 10 years after entry)
- Institutional characteristics and geographic regions

## Data Cleaning Steps
1. Removed institutions with missing or invalid SAT score or earnings data
2. Standardized variable names and formats across years
3. Filtered to institutions with sufficient reporting coverage
4. Aggregated and aligned SAT and earnings variables to ensure comparability

### Research Question
1. Do higher average SAT scores predict higher post-graduation earnings at U.S. universities?
2. Does the relationship between SAT scores and earnings vary across geographic regions in the United States?

### Analysis and Visualization Techniques: 
- Descriptive statistics by region
- Exploratory data analysis (histograms, scatter plots, trend lines)
- Bayesian hierarchical linear regression
- Markov Chain Monte Carlo (MCMC) sampling
- No-U-Turn Sampler (NUTS) for improved convergence
- Posterior diagnostics including trace plots and autocorrelation analysis

## Authors
Yoonseo Bae, Vivian Liu, Riddhi Bharj
