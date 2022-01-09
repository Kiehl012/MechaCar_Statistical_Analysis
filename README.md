# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG </br>
![Screen Shot 2022-01-09 at 12 44 36 PM](https://user-images.githubusercontent.com/90878911/148696121-0f3c374d-8396-42d9-9809-f734fd160a32.png)</br></br>

Based on the summary results for this model, we can say that vehicle length, ground clearance, and the intercept have a statistically significant relationship among the 50 MechaCar prototype in our data set. This is based on a confidence level of < 0.05. However, we could not conclude a non-random relationship between gas mileage and vehicle weight, spoiler angle, and AWD (boolean). Based on a multiple R-squared value of 0.7149, this model explains roughly 72% of the variation in gas mileage among the 50 protoypes. With this, we can conclude that the model effectively predicts mpg of MechaCar prototypes, but with multiple 'insiginificant' variables, this model may be overfit for our data set. </br></br>

## Table 1: Summary Statistics on Suspension Coils

#### Table 2: Suspension Coil PSI (pounds per square inch) Data for All Manufacturing Lots
![Screen Shot 2022-01-09 at 1 54 40 PM](https://user-images.githubusercontent.com/90878911/148698580-092fdac5-04ac-47f8-96cf-585a4707fd3a.png)

#### Suspension Coil PSI (pounds per square inch) Data by Manufacturing Lot
![Screen Shot 2022-01-09 at 1 54 48 PM](https://user-images.githubusercontent.com/90878911/148698578-e650bb24-4e7d-4bfc-ab74-5e2c179d5292.png) </br></br>

Looking at the first table above, the variance of suspension coil PSI meets the requirement of 100 PSI or less. However, when we break this summary down by manufacturing lot (table 2), we can see that lot three has far exceeded the 100-pound allowance, while lots 1 and 2 are well within the allowed variance. </br></br>

## T-Tests on Suspension Coils
#### All Lots
![Screen Shot 2022-01-09 at 2 57 32 PM](https://user-images.githubusercontent.com/90878911/148700808-ab28b31d-71ca-4922-b9bc-a43090c258d1.png)
#### Lot 1
![Screen Shot 2022-01-09 at 2 57 42 PM](https://user-images.githubusercontent.com/90878911/148700812-bdc8671d-f940-43c0-aa8a-347efe99c7db.png)
#### Lot 2
![Screen Shot 2022-01-09 at 2 57 57 PM](https://user-images.githubusercontent.com/90878911/148700817-1dd7982e-d557-43ed-92a7-7e261b61365e.png)
#### Lot 3
![Screen Shot 2022-01-09 at 2 58 16 PM](https://user-images.githubusercontent.com/90878911/148700819-3801439b-4dc3-4c41-aa60-499720b5e0ac.png)</br>

Given the t.test results above we can make conclude that:
1. Using a significance level of < 0.05, there is no statistically significant difference between the mean PSI of our total sample data and a population mean of 1500 PSI.
2. Using a significance level of < 0.05, there is no statistically significant difference between the mean PSI of coils from Lot1 and a population mean of 1500 PSI.
3. Using a significance level of < 0.05, there is no statistically significant difference between the mean PSI of coils from Lot2 and a population mean of 1500 PSI.
4. Using a significance level of < 0.05, there is a statistically significant difference between the mean PSI of coils from Lot3 and a population mean of 1500 PSI.</br><br>

## Study Design: MechaCar vs Competition
#### Overview
For this study, let's assume that MechaCar produces high-end EVs. In high-end EVs, performance is often a major draw. Specifically, consumers and EV manufacturers alike are often very focused on the time it takes for the vehicle to accelerate from 0-60 miles per hour. So, a good way to compare MechaCar EVs to EVs from other manufacturers would to see how it's 0-60 time stacks up against the competition. However, it's important to make sure that the comparison's make sense. For example, if the given MechaCar model is a 4-door sedan, then it doesnt make sense to compare it to a Audi SUV EV. For the sake of this experiment, we will say that Tesla and Audi are the main EV competitors.</br>

#### Hypotheses:
Null Hypothesis: There is no difference between the 0-60 time of the MechaCar EVs and Tesla and Audi EVs.
Alternative Hypothesis: There is a statistically significant difference between the 0-60 time of the MechaCar EVs and other manufacturers.</br>

#### Statistical Test:
Given that there are multiple manufacturers, it might seem like an ANOVA test would be a good fit, but we really want to compare MechaCar to the other manufactures, rather than how all three groups compare to each other. With this in mind, it makes more sense to us t-tests to compare 0-60 times of MechaCars to similar vehicles made by Tesla and Audi. This will tell help describe how MechaCar stacks up against both competitors individually.</br>

#### Data Needed
In order to perform this experiment, EV data is needed from each manufacturer. Specifically, we will need the model, vechicle class, drive type (awd, fwd, rwd etc.) and 0-60 time for each model from each manufacturer. Variables like vehicle class and drive type are there to ensure we are comparing similar vehicles across manufacturers.






