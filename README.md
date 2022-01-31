# MechaCar_Statistical_Analysis

## Background

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:

- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Deliverable 1: Linear Regression to Predict MPG

The linear regression model I created predicts MPG of MechaCar prototypes by using vehicle weight and length, spoiler angle, ground clearance and if it has AWD or not.
Here are my results:
<img src="Resources/Dev1_linear_regression.PNG">

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Coefficients vehicle length and ground clearance are statistically mopre likely to generate non-random amounts of variance. This means those two variables are highly impactful to the MPG on the MechaCar.  The other variables have p-values that suggest they have a randion amount of variance with the dataset.

### Is the slope of the linear model considered to be zero? Why or why not?
The slope of the linear model is not considered to be zero because the p-value is less than 0.05. 

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
This model has an r-squared value of 0.7149 which means this regression model does predict the MPG of MechaCar accurately 71% of the time.


## Deliverable 2: Create Visualizations for the Trip Analysis

Here is what the total summary for manufacturing lots looks like: <br/>
<img src="Resources/total_lot_summary.png"> <br/>

Here is a deeper dive into each of the lots: <br/>
<img src="Resources/total_lot_summary_breakdown.png"> <br/>


The results of this data analysis on the 3 lots show that lots 1 & 2 meet the design specifications because they are under 100 lbs/sq in. but lot 3 does noit since it is above 100.

## Deliverable 3: T-Tests on Suspension Coils

T-test across all lots: <br/>
<img src="Resources/Dev3_ttest_all_lots.PNG"> 

T-test across each individual lot : <br/>
<img src="Resources/Dev3_ttest_lot1.PNG">
<img src="Resources/Dev3_ttest_lot2.PNG">
<img src="Resources/Dev3_ttest_lot3.PNG">

### Analysis Summary
- Lot 1: We cannot reject the null hypothesis because there is no statistically difference between the observed sample and presumed population mean.
- Lot 2: We cannot reject the null hypothesis.
- Lot 3: P-value is .04 so this indicates to reject the null hypothesis.


## Deliverable 4: Study Design: MechaCar vs Competition

## What metric or metrics are you going to test?
Independent variable:
- Safety Feature Rating
- Drive Package
- Engine
- Resale Value
- Average Annual Cost of ownership 
- Gasoline Efficiency)

Dependent Variable
- Current Price


## What is the null hypothesis or alternative hypothesis?
Null hypothesis: MechaCar is priced correctly.

Alternative hypothesis: MechaCar is not priced correctly.

## What statistical test would you use to test the hypothesis? And why?
T-test because we showed its usefulness above.

## What data is needed to run the statistical test?
A table of MechaCar data.
