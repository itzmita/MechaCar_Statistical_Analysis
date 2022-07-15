# MechaCar_Statistical_Analysis
Learning Statistics and R
## Project Overview:

AutosRUs is developing a new prototype vehicle, MechaCar which is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.


## Linear Regression to Predict MPG

![image](https://user-images.githubusercontent.com/3753839/179283035-70910f31-99b9-431c-8d84-f7dacba66435.png)

* From the above results we can see that the following variables contributed non-random amount of variance to the mpg values:
  * Vehicle_length(2.60e-12) 
  * ground_clearance (5.21e-08)
    
  Probability value or the p-value from the above variables are seen to be extremely less. The low p-value suggests that the results are more constant. That means that   they have high significance value. 
  
* This is because the p-value for this linear model is 5.35e-11 which is much less than assumed significance value of 0.05. Which suggests that there is enough evidence to reject the null hypothesis and hence the slope of the linear model is not considered to be zero.
  
* As per the summary shown above, we can see that the r-squared value is 0.7149, which says that approx 71% of all mpg predictions will be correct when using this linear model which can be considered effective enough but it can be made better.
 

## Summary Statistics on Suspension Coils
Total Summary DataFrame 

![image](https://user-images.githubusercontent.com/3753839/179283110-e4406377-df19-4efc-b8de-10f3b9fc1c56.png)

Lot Summary DataFrame

![image](https://user-images.githubusercontent.com/3753839/179283151-c97be2ba-e51e-4757-94b4-f2eb97f54278.png)

• The overall variance, as shown in the Total Summary dataFrame above, is under 100 PSI and hence meets the specifications. If we see variance for Lot1 it is 0.97 which is also under 100 PSI. Same for Lot2 as well which is 7.46 and meet the specification. However Lot3 shows a variance of 170.28 which is more than the specified level 100. 


## T-Tests on Suspension Coils

Suspension Coils Cumulative T-test shown as below tells us that the true mean is 1498.78 which means that the mean of all the 3 Lots are similar to the assumed mean of 1500. And the p-value is 0.06 which is slightly more than 0.05 so its not enough evidence to reject the null hypothesis.

![image](https://user-images.githubusercontent.com/3753839/179284885-29472155-fb22-4329-a9e7-e4efde2d0e53.png)


Lot1 T-test shown as below tells us that the mean of this Lot is 1500 which says there is no statistical difference with the population mean. Also the p-value is 1 which is again more than 0.05 so its not enough to reject the null hypothesis.

![image](https://user-images.githubusercontent.com/3753839/179285119-4b8a0b4d-fda5-4aed-a283-2617cd3f1b97.png)


Lot2 T-test shown as below tells us that the mean of this Lot is 1500.2 which says there is no statistical difference with the population mean. Also that the p-value is 0.06 which is again slightly more than 0.05 so its not enough to reject the null hypothesis.

![image](https://user-images.githubusercontent.com/3753839/179284988-42a81eca-622b-4a3e-817d-fa88d8488ee5.png)

Lot3 T-test shown as below tells us a little different story. The mean of this Lot is 1496.14 which says there is a slight statistical difference with the population mean. Also that the p-value is 0.4168 which is just less than 0.05 and its just enough to reject the null hypothesis.	

![image](https://user-images.githubusercontent.com/3753839/179285035-dc118b8e-7683-446f-9ec6-f2b5bcdcf1d0.png)


As seen above, we may want to check the Lot3 manufacturing process more deeply as the results are slightly different from the other Lots and also the population. 


## Study Design: MechaCar vs Competition

A statistical study that can quantify how the MechaCar performs against the competition. In our study design, we are thinking about metrics that would interest consumers and motivate them to buy MechaCar vehicles based on data.


• We are going to test on city or highway fuel efficiency for Mecha car and a hybrid car for example.

• H0: Test drive of 20 miles in the MechaCar prototypes' and with a hybrid car with 1 gallon of Fuel will not show any difference.
Ha: Test drive of 20 miles in the MechaCar prototypes' and with a hybrid car with 1 gallon of Fuel will show difference in mpg.

• The best statistical test for this would be two-sample t-tests. One population would be from the Mecha car data and the other population would be from the hybrid car. We can compare and see if the true mean for Mecha car is more than the hybrid car. Also we can check the p-value if < 0.05 in which case it will be a successful test and reject the null hypothesis

• Fuel consumed and distance travelled are the factors needed to run a statistical test to see how it impacts the mpg for both the cars in this example.





