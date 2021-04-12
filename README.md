# MechaCar_Statistical_Analysis-

## Linear Regression to Predict MPG
For our linear regression model, we used the following hypotheses and significance level:
- H0 : The slope of the linear model is zero, or m = 0
- Ha : The slope of the linear model is not zero, or m ≠ 0
- Significance Level: 0.05

![lm](/resources/lm.PNG)

![lm_summary](/resources/lm_summary.PNG)

- From our analysis, we determined that the intercept, vehicle length and ground clearance are statistically unlikely to provide random amounts of variance to the mpg values in the dataset.

- Our p-value is 5.35e-11, which is significantly lower than our assumed significance level of 0.05%. This means that there is enough evidence to reject our null hypothesis and assume that the slope of the linear model is not zero.

- Our multiple r-squared value is 0.7149. This tells us that roughly 71.5% of all mpg predictions will be correct when using this linear model.

## Summary Statistics on Suspension Coils

![total_summary](/resources/total_summary.PNG)

Based on our results, we can see that the pounds per square ince (PSI) variance is 62.29, which meets design specifications. 

![lot_summary](/resources/lot_summary.PNG)

However, when we break the results down by lot, we can see that lot 3 fails to meet design specifications, as the variance is 170.29, which is exceeds the 100 pounds per square inch limit.

## T-Tests on Suspension Coils

We used the following hypotheses and significance level for our t-Tests:
- H0 : There is no statistical difference between the two means.
- Ha : There is a statistical difference between the two means.
- Significance Level: 0.05

### T-Test: All Manufacturing Lots
- Our p-value is 0.06 which is higher than our significance level. Therefore our null hypothesis passes and we can conclude that the two means are similar.

![ttest1](/resources/ttest1.PNG)

### T-Test: Lot 1
- Our p-value is 1.00 which is higher than our significance level. Therefore our null hypothesis passes and we can conclude that the two means are similar.

![ttest2](/resources/ttest2.PNG)

### T-Test: Lot 2
- Our p-value is 0.61 which is higher than our significance level. Therefore our null hypothesis passes and we can conclude that the two means are similar.

![ttest3](/resources/ttest3.PNG)

### T-Test: Lot 3
- Our p-value is 0.04 which is lower than our significance level. Therefore our null hypothesis fails and we can conclude that the two means are not similar.

![ttest4](/resources/ttest4.PNG)

## Study Design: MechaCar vs Competition
One of the main metrics that would be of interest to a consumer when choosing a car is affordability, so in this study I have chosen to focus on how cost affects the consumer's decision to choose MechaCar over its competition. 

The following hypotheses and significance level will be used for our tests:
- H0 : Cost does not affect the consumer's decision to choose MechaCar over its competitors.
- Ha : Cost does affect the consumer's decision to choose MechaCar over its competitors.
- Significance level: 0.05

Since we will be analysing how cost impacts the consumer's behaviour in MechaCar's many competitors, we will need to use a statistical test that allows us to determine if there is a statistical difference in the means from multiple samples. Therefore, we will be using the ANOVA test.

To preform this test, we will need the following data:
- Cost will be our dependent, continuous variable.
- The manufacturer will be our independent, categorical variable.
- Household income will also be used as an independent, categorical variable when analysing the consumers' spending power.
