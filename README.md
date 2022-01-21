# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

After running a linear regression model on the data, it appears that the variables/coefficents of the vehicle length and the vehicle ground clearance provided non-random amounts of variance to the mpg values in the dataset. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset.

The p-value is 5.35e-11 (0.0000000000535) which is less than the significant level of 0.05. Due to this, the slope is not equal to zero and there is sufficent statistical evidence to reject the null hypothesis.

The r-squared value of this model is 0.7149. This indicates that approximately 72% (if rounded) of all predictions of the mpg of MechaCar prototypes will be correct.

![lm](Resources/lm.png)

![lmsum](Resources/lmsum.png)

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch (PSI). From the below image that examines all 3 lots, we can see that the suspension coils have a variance of 62.29356 PSI. This is within the requirement for the variance not exceeding 100 PSI.

![total](Resources/total.png)

When looking at each of the 3 lots individually however, we can see that Lot 3 shows a significantly higher variance than Lots 1 and 2. Lot 3's variance at 170.2861224 far exceeds the 100 PSI mandate. Meanwhile, the variance in Lots 1 and 2 are much closer in number and appear to be on the opposite side of the variance spectrum. Therefore, we can safely conclude that Lot 3 is disproportionally affecting the variance level when looking at the lot data together as a whole.

![lot](Resources/lot.png)

## T-Tests on Suspension Coils
A T-Test of the suspension coils was also performed on the lots as a whole.  The goal was to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 PSI. The T-Test performed on all three lots resulted in a p-value of 0.06, which is higher than the significance value of 0.05. This indicates that there is not enough evidence to reject the null hypothesis, thus we fail to reject the null hypothesis. Additionally, the mean is 1498.78, which is just under the population mean of 15000 PSI. As such, the PSI across all manufacturing lots is NOT statisically differenet from the population mean.

![ttest](Resources/ttest.png)

Additionally, T-Tests were performed on each individual lot. The goal of these T-Tests were to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 PSI. This resulted in a p-value higher than the significance level for for Lots 1 and 2, but a lower p-value than the significance level for Lot 3. The sampled mean for all three were very close to the population mean of 1500 PSI. Lot 1's mean was exactly the same, Lot 2's mean was ever-so-slightly above, and Lot 3's mean was still relatively close. In conclusion, this means the PSI for each manufacturing lot is NOT statisically different from the population mean. See the below image for a detailed breakdown: 

![lotttest](Resources/lotttest.png)

## Study Design: MechaCar vs Competition
There are many factors/variables that can and should be analyzed when comparing how MechaCar would stack up to the competition. These metrics include the cost of the car, city or highway fuel efficiency, horse power, maintenance cost, and safety rating. Since there are so many variables to test for, it would be recommended to use an ANOVA test. An ANOVA test would test for the means of each category and also reveal if the p-values for each variable is above or lower than the 0.05 significance level threshold.

The null hypothesis that would be proposed would be that MechaCar is on par with the competition based on having similar statistics in these categories of metrics. The alternative hypothesis is that MechaCar is NOT on par with the competition. 
