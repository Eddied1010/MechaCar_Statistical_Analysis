# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

Summary:
lm(formula = mpg ~ vehicle_length + vehicle_weight + spoiler_angle + 
    ground_clearance + AWD, data = mechacar_table)

Residuals:
     Min       1Q   Median       3Q      Max 
-19.4701  -4.4994  -0.0692   5.4433  18.5849 

Coefficients:
                   Estimate Std. Error t value
(Intercept)      -1.040e+02  1.585e+01  -6.559
vehicle_length    6.267e+00  6.553e-01   9.563
vehicle_weight    1.245e-03  6.890e-04   1.807
spoiler_angle     6.877e-02  6.653e-02   1.034
ground_clearance  3.546e+00  5.412e-01   6.551
AWD              -3.411e+00  2.535e+00  -1.346
                 Pr(>|t|)    
(Intercept)      5.08e-08 ***
vehicle_length   2.60e-12 ***
vehicle_weight     0.0776 .  
spoiler_angle      0.3069    
ground_clearance 5.21e-08 ***
AWD                0.1852    
---
Signif. codes:  
0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 8.774 on 44 degrees of freedom
Multiple R-squared:  0.7149,	Adjusted R-squared:  0.6825 
F-statistic: 22.07 on 5 and 44 DF,  p-value: 5.35e-11          

In summary, some variables does significantly impact the mpg as others does not. From our linear regression model, the r-squared value is 0.715, which means that roughly 70% of the variablilty of our dependent variable (mpg predictions) is explained using this linear model. 

In addition, the p-value of our linear regression analysis is 
 Vehicle Length  - 2.60 x 10-12 - smaller than significance level of 0.05%
 vehicle weight - 0.0776 - Strong significance
 spoiler Angle - 0.3069 - very weak
 Ground Clearance - 5.21e-08 - smaller than significance level of 0.05%
 All-Wheel Drive(AWD) - 0.1852 - Strong signifance.

 Therefore, we can state that there is sufficient evidence to reject our null hypothesis, which means that the slope of our linear model is not zero for Vehicle Length and Ground Clearance. However, for variables vehicle weight and AWD there is a higher correlation between these values that can explain/predict the value of mpg.
