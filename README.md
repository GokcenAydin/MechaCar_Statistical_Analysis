# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

In the first part of the analysis was based on MechaCar_mpg dataset which was containing the mpg test results of 50 prototype MechaCars.
Various design qualifications were used to create the MechaCar prototypes. Using these variables from the dataset, a multiple linear model that 
predicts the mpg of the MechaCar prototypes was designed by using R. In the multiple linear model, the predictors were vehicle length, vehicle weight,
spoiler angle, ground clearance and AWD, compared to mpg values in the dataset. 

![Part1](https://user-images.githubusercontent.com/104400293/206830215-a438968a-3baf-4427-bb9c-4140231844ca.PNG)

- Vehicle length and ground clearance provided a non-random amount of variance to the mpg values in the dataset as their significance levels are lower
than and equal to 0.05, which is within normal levels.
- The slope of the linear model is considered to be non-zero as the intercept has a probability which is quite less than 0.5.
- This linear model predicts mpg of MechaCar prototypes effectively as multiple R-squared value is 0.7149, which is closer to 1 than it is closer to 0. 

## Summary Statistics on Suspension Coils

In the second part of the analysis, using the Suspension_coil dataset which contains the results from multiple production lots, the weight capacities of
multiple suspension coils were tested to determine if the manufacturing process is consistent across procution lots. Lot summary table showing mean,
median, variance and standard deviation for each lot and total summary statistics table showing the suspension coil's PSI continuous variable across all
manufacturing lots were created in this part of the analysis. 

![Lot_Summary](https://user-images.githubusercontent.com/104400293/206830226-97e867db-a041-4ce4-815f-6753037d7966.PNG)

![Total_Summary](https://user-images.githubusercontent.com/104400293/206830236-0710401e-084a-4e22-8285-eb21d48e02ba.PNG)

-The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not 
exceed 100 pounds per square inch. In this case, the current manufacturing data meets this design specifications if you consider all lots in total as the 
variance of the total summary of all lots is less than 100 pounds. 
However, when the lots are considered individually, only Lot 1 and Lot 2 are within 100 pounds where they meet the design specifications, but variance of Lot 3 
is 170, which is above 100 and for this reason, does not meet the design specifications. 

## T-Tests on Suspension Coils

In the third part of the analysis, a t.test function for overall manufacturing lots; and in the following step, three more RScripts were written using the same function and its subset
argument to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1500 pounds per square inch.
The mean value of all manufacturing lots is 1498.78 and Lot 3 is 1496.14, which are lower than 1500, which means that they are significantly different from the population mean of 1500; 
wheras the mean value of Lot 1 is 1500 and Lot 2 is 1500.2, which are higher than and equal to 1500, which means they are not significantly different from the population mean of 1500.  

![All_t_test](https://user-images.githubusercontent.com/104400293/206830262-4827eec6-5a80-46f4-ac07-75454b6e2417.PNG)

![Lot1_t_test](https://user-images.githubusercontent.com/104400293/206830266-4c780803-7605-433e-9ae4-57a99cabdd83.PNG)

![Lot2_t_test](https://user-images.githubusercontent.com/104400293/206830269-25c96eae-2a30-48bd-9f96-3e6e7c11a71a.PNG)

![Lot3_t_test](https://user-images.githubusercontent.com/104400293/206830272-f3022850-e5fb-4f1d-b16c-586369d6cf67.PNG)

## Study Design: MechaCar vs Competition

In my statistical study that will quantify how the MechaCar performs agains the competition, the points below will be considered:

- City or highway efficiency is going to be tested. 
- My research question is "Does lower ground clearence of a light-weighed automobile cause safety risks of accidents for drivers due to the risk of getting caught on low 
obstacles while driving?"
Null hypothesis is "Lower ground clearence has no effect on the rate of car accidents." The explanation is that ground clearence has no direct effect of the cause of the car 
accidents, as the numbers and natures of the accidents are considered, there are many other reasons causing the accidents directly.
Alternative hypothesis is "Lower ground clearence has an effect on the number of car accidents in light-weighted." The explanation for the this hypothesis is that, 
lower ground clearence affects driving safety in an indirect way with reasons like getting caught on a low obstacle, losing concentration and control of the wheel, 
which causes an accident -especially because the light weighted cars are weaker in balance and endurance.
- I would use a t.test to test the hypothesis in order to see the if p-values of each model are over 0.05, which is the normal value, and the mean values are statistically different 
from the population mean of 1500 pounds per square inch.
- The cause of accident rates in certain models of cars and ground clearence information of these cars are needed to run the statistical test. 
