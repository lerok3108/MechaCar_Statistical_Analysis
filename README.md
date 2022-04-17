# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG
![image](https://user-images.githubusercontent.com/96098938/163720881-e86205f0-9ba1-44be-abc9-aa8dc74f5610.png)
Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
* The most significant variables in our dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. As observed in the image above, a linear regression model run on these variables a resulted in p-values of 2.6x10-12 and 5.21x10-8, respectively. The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the MPG.
Is the slope of the linear model considered to be zero? Why or why not?
* The slope of the linear model can not be considered to be zero, as the p-value of 5.35x10-11 is lower than even an extreme level of significance, and thus the null hypothesis must be rejected. This means that the relationship between our variables and the miles per gallon is subject to more than random chance

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
* Although there are still  factors we have not considered, this model does predict the mpg of the MechaCar prototype with some level of effectiveness. The r-squared value of 0.7149 indicates that the model is 71% accurate.

## Summary Statistics on Suspension Coils
Total Summary
![image](https://user-images.githubusercontent.com/96098938/163721175-49619460-8f7f-42dd-9539-1f9c2389acfb.png)

Lot Summary
![image](https://user-images.githubusercontent.com/96098938/163721139-f07e0e2e-de7a-46d2-8cde-3921b6395824.png)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
* While the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications, there is a problem with one of the lots. As shown in the Lot Summary results, the variance for Lot 3 is well over the acceptable threshold, at 170.28.


## T-Tests on Suspension Coils
Results of one sample t-test
![image](https://user-images.githubusercontent.com/96098938/163721369-eed88646-9835-4c19-9617-3a9a61c54c84.png)
T-testing 3 different lots
![image](https://user-images.githubusercontent.com/96098938/163721586-b753d45a-8807-43d6-9bfa-3cd8a6266640.png)
Summary
* A review of the results of the T-test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value is not low enough (0.0603) for us to reject the null hypothesis.
* A review of the results of the T-test for the suspension coils for Lot 1 shows that they are not statistically different from the population mean, and the p-value is not low enough (1) for us to reject the null hypothesis.
* A review of the results of the T-test for the suspension coils for Lot 2 shows that they are not statistically different from the population mean, and the p-value is not low enough (0.6072) for us to reject the null hypothesis.
* A review of the results of the T-test for the suspension coils for Lot 3 shows that they are statistically different from the population mean, and the p-value is  low enough (0.0417) for us to reject the null hypothesis. This lot may be need to be discarded, or evaluated further. 


## Study Design: MechaCar vs Competition
The proposed study would compare safety and price of the MechaCar vehicles in relation to the other vehicles on the market
* What metric or metrics are you going to test?
 Overall Safety Rating: Safety Ratings are available at https://www.nhtsa.gov/ratings. The ‘overall’ category is made up of various sub-categories like: Frontal Crash, Side Crash, Rollover, etc.; but we just need a categorical ‘overall safety rating’ (e.g. A, B, C, D, E, and F)
Price of MechaCar vehicles and other vehicles we want to comapare. 
* What is the null hypothesis or alternative hypothesis?
Null hypothesis-There is no correlation between price and safety of vehicles
 Alternative hypothesis-more expensive vehicles are safer
* What statistical test would you use to test the hypothesis? And why?
In order to establish correlation, the Pearson correlation test will be used. This test will be able to establish if there is cause-and-effect relationship between these 2 variables
* What data is needed to run the statistical test?
In order to run this test, we will need to collect prices for the vehicles we want to compare and collect overall safety ratings. Both data is easily available.

