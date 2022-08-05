# MechaCar

CWRU Data Analytics Module Fifteen Challenge


## Overview of Project

The project involved utilizing R to perform statistical analysis on data regarding the MechCar and the dependent/indepent variables which relate to mpg and three production lots of suspension coils used in the vehicles.  

### Summary

The effort involved using R to load datasets regarding mpg and suspension coil lots.  Linear regression was performed on the MechCar attributes in relation to mpg.   Summary statistics and t-tests to determin lot variance vis-a-vis specifications was performed on the suspension coil data. T For each deliverable a specific set of questions to be answered were specified.  echnial analysis and written summary for each of four deliverables are outlined below:   

## Major components of the work:
-------------------------------------------------------------------------
### Deliverable 1: Linear Regression to Predict MPG 
This deliverable involved loading the data, performing linear regressions and three questions to answer were specified:

* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

* Is the slope of the linear model considered to be zero? Why or why not?

* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?


### Deliverable 2: Create Visualizations for the Trip Analysis
This deliverable involved creating summary a summary statistics table to show 
(a) The suspension coil’s PSI continuous variable across all manufacturing lots; and
(b)  PSI metrics for each lot: mean, median, variance, and standard deviation.   The following question was posed to answer:

* The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?


### Deliverable 3: T-Tests on Suspension Coils
This deliverable involved performing t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

* The question here is to briefly summarize interpretation and findings for the t-test results

### Deliverable 4: T-Tests on Suspension Coils
This deliverable involved designing a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.  Four questions were posed: 

* What metric or metrics are you going to test?
* What is the null hypothesis or alternative hypothesis?
* What statistical test would you use to test the hypothesis? And why?
* What data is needed to run the statistical test?

## Linear Regression to Predict MPG (Deliverable 1) 

Linear regression on factors related to MPG produces the following result: 

![img](https://github.com/fhsal/MechaCar/blob/main/images/Deliverable1_LinearRegressionOutput.png)

Statistical summary of the linear model are below and indicate that vehicle length and ground clearance are the independent variables with non-zero variance that contribute to MGP.  The p-value is far below significance, indicating that the null hypothesis can be rejected and the slope of the linear model is non-zero: 

![img](https://github.com/fhsal/MechaCar/blob/main/images/Deliverable1_LR_Summary.png)


## Summary Statistics on Suspension Coils (Deliverable 2)

Statistical summary of the coils and three lots are below and indicate that the overall group falls within the quality tolerance for variance of +/- 100, but the third lot does not as it shows a variance of 170 PSI. 

### Overall summary

![img](https://github.com/fhsal/MechaCar/blob/main/images/coil_total_summary.png)

### Lot summary

![img](https://github.com/fhsal/MechaCar/blob/main/images/coil_lot_summary.png)


## T-Tests on Suspension Coils (Deliverable 3)

T-Tests of the coils and three lots are below and indicate that the p-value for the overall group is above the significance level of .05 and we cannot reject the null hypothesis, meaning that the total group falls within the population mean of 1500. 

### Overall T-Test

![img](https://github.com/fhsal/MechaCar/blob/main/images/coil_total_summary.png)

### Lot 1 T-Test

![img](https://github.com/fhsal/MechaCar/blob/main/images/Lot1_T-Test.png)

### Lot 2 T-Test

![img](https://github.com/fhsal/MechaCar/blob/main/images/Lot2_T-Test.png)

### Lot 3  T-Test

note variance of 170, above the quality threashold of 100

![img](https://github.com/fhsal/MechaCar/blob/main/images/Lot3_T-Test.png)


## Study Design: MechaCar vs Competition (Deliverable 4) 

Although there are any number of attributes one could compare MechaCar to its competitors on, the most obvious competitive test given this analysis here would be to focus upon the factors in those vehicles which similarly drive MPG.   It may very well be that there are other factors in those vehicles which drive improvements in MPG that MechaCar hasn't yet identified that are not currently within this dataset and/or analysis.   

In that regard, the metrics which might be considered (independent variables) as influencing MPG (dependent variable) could include:

* Engine size
* Tire size
* Transmission type
* Vehicle frontal area

The hypothesis would be:

* Null:  The factors which drive MPG for MechaCar are the same as the competition 

* Alternative:  The competition has used one or more of the factors to impact MPG in a way that is statistically significantly different 

The Statistical tests to run would likely be a series of statistical regression to detmine wich factor(s) differentiate MechaCar MPG from its competition 



