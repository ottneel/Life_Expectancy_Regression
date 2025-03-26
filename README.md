# Life Expectancy Prediction Project
## Overview

This project uses multiple linear regression to predict life expectancy based on socioeconomic and health-related factors. The model identifies key drivers of longevity and evaluates their impact, providing actionable insights for public health policy.
## Key Findings
**1. Model Performance**  

A. R² (Training): 0.9759 → Model explains 97.6% of variance.  
B. R² (Test): 0.9708 → Strong generalization to unseen data.  
C. MAE (Test): 1.19 years → Predictions are off by ~1.2 years on average.  
D. RMSE (Test): 1.56 → Low error relative to life expectancy range (50–90 years).  

**2. Top Predictors of Life Expectancy**   
A. Economy_status_Developed	with +0.80 coefficient:	Developed nations add 0.8 years to life expectancy.  
B. Schooling with	+0.10	coefficient: Each additional year of education adds 0.1 years.  
C. Under_five_deaths with	-0.07 coefficient:	Each unit increase reduces life expectancy by 0.07 years.  
D. Adult_mortality with	-0.05 coefficient:	Each unit increase reduces life expectancy by 0.05 years.  
E. Polio with	-0.03 coefficient:	Requires investigation.  

**3. Assumptions Validated**  
A. Linearity: Confirmed via scatterplots (most features).  
B. Multicollinearity: Addressed with Ridge regression (L2 penalty).  
C. Outliers: Clipped at 1.5×IQR.  
D. Residuals: Near-normal distribution (minor deviations in Q-Q plot).  

## Conclusions & Recommendations  
1. Prioritize Economic Development: The strongest predictor (+0.80 years).  
2. Invest in Education: Schooling has a clear, measurable impact (+0.10/year).  
3. Reduce Child Mortality: Under-five deaths are disproportionately impactful (-0.07/unit).  
4. Investigate Polio’s Negative Coefficient: Likely reflects regional healthcare disparities, not vaccine inefficacy.  
   
