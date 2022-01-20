# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

After running a linear regression model on the data, it appears that the variables/coefficents of the vehicle length and the vehicle ground clearance provided non-random amounts of variance to the mpg values in the dataset. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset.

Is the slope of the linear model considered to be zero? Why or why not?
The p-value (5.35e-11) is less than the significan the slope is not equal to zero

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
The r-squared value of this model is 0.7149. This indicates 

![lm](Resources/lm.png)

![lmsum](Resources/lmsum.png)

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

![total](Resources/total.png)

![lot](Resources/lot.png)

## T-Tests on Suspension Coils
briefly summarize your interpretation and findings for the t-test results.

![ttest](Resources/ttest.png)

![lotttest](Resources/lotttest.png)

## Study Design: MechaCar vs Competition
Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.

In your description, address the following questions:
What metric or metrics are you going to test?
What is the null hypothesis or alternative hypothesis?
What statistical test would you use to test the hypothesis? And why?
What data is needed to run the statistical test?
