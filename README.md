# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG
    
The MechaCar_mpg.csv dataset contains mpg test results of 50 prototype,which were produced using multiple design specifications to identify ideal vehicle performance across multiple variables.

### Linear Regression 
   The linear regression was calculated using R in R Studio(R 4.1.2).The R script was applied to the dataset on several variables to get the following coefficients.
   A summary of the linear regression can be displayed to determine the quality of data set.
   
   ![Deli_1_summarystatistics.png](Resources/Images/Deli_1_summarystatistics.png)
  
   
1) Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Coefficients:
  mpg: 0 < .05,Statistically significant,non-random amount of variance
  Vehicle length:   0 < .05,   Statistically significant,non-random amount of variance
  Vehicle weight:  .08 > 0.05,  Not statistically significant,random amount of variance
  Spoiler angle:   .31 > 0.05, Not statistically significant,random amount of variance
  Ground Clearance: 0 > .05   Statistically significant, non-random amount of variance
  AWD:             .19>=.05 Not statistically significant,random amount of variance
  
  In summary, vehicle length and ground clearance variables represent non-random amountsof variance as applied to the mpg values.

2) Is the slope of the linear model considered to be zero? Why or why not?

   By converting to scientific notation, all of the slopes of the variables are shown  to be non-zero,some close to zero
   
   Coefficients:
   
  Vehicle length(vl):  6.267
  Vehicle weight (vw):  .001
  Spoiler angle (sa):    .069
  Ground clearance(gc):  3.546
  AWD (awd):              -3.411
  
  The multiple linear regression formula for mpg = -.01+6.267(vl)+ .001(vw)+.069(sa)+3.546(gc)-3.411(awd) which results in a non-zero slope
      
   

3) Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
