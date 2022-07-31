#                Regression-Satisfaction


##  Does Delivery Speed improve Satisfaction?

![image](https://user-images.githubusercontent.com/104678755/182026292-133fb405-918d-4483-8f90-9bd09ba0e9b0.png)


Coefficients:
                Estimate Std. Error t value Pr(>|t|)    
 (Intercept)      3.2791     0.5294   6.194 1.38e-08 ***
 Delivery.Speed   0.9364     0.1339   6.994 3.30e-10 ***


 Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
 
 Residual standard error: 0.9783 on 98 degrees of freedom
 Multiple R-squared:  0.333,  Adjusted R-squared:  0.3262 
 F-statistic: 48.92 on 1 and 98 DF,  p-value: 3.3e-10
 
 
 #              What about the interaction of Delivey Speed and Location?
 
 ![image](https://user-images.githubusercontent.com/104678755/182026407-36cd8674-7c2b-44bc-af01-87b64c0db3d2.png)


#              Let’s compare the results using Texreg (Alternative: Stargazer)

=============================================================================
##                                          No interaction            Interactio
                                ----------------------------------  ----------
                                M1          M2          M3          M4        
 -----------------------------------------------------------------------------
 Delivery.Speed                    .94 ***     .36         .40         .70 ** 
                                  (.13)       (.22)       (.21)       (.23)   
 Quality.percption                             .40 ***     .38 ***     .38 ***
                                              (.06)       (.06)       (.05)   
 E.Commerce.experience                         .36 **      .37 **      .43 ***
                                              (.12)       (.12)       (.11)   
 Technical.support.perception                 -.01         .04        -.00    
                                              (.08)       (.08)       (.08)   
 Complaint.resolution                          .27 *       .32 *       .32 *  
                                              (.13)       (.13)       (.12)   
 Advertising.perception                        .13         .10         .07    
                                              (.08)       (.07)       (.07)   
 Competitive.pricing                          -.01        -.01        -.04    
                                              (.06)       (.05)       (.05)   
 Warranty                                      .09         .00         .07    
                                              (.16)       (.15)       (.15)   
 Ordering.process                              .04        -.04        -.12    
                                              (.13)       (.13)       (.13)   
 LocationSuburb                                           -.47 **     1.74 *  
                                                          (.16)       (.81)   
 Delivery.Speed:LocationSuburb                                        -.57 ** 
                                                                      (.21)   
 (Intercept)                      3.28 ***   -1.49        -.89       -1.82    
                                  (.53)      (1.06)      (1.04)      (1.05)   
 -----------------------------------------------------------------------------
 R^2                               .33         .65         .68         .71    
 Adj. R^2                          .33         .61         .65         .67    
 Num. obs.                      100         100         100         100       
 =============================================================================
 *** p < 0.001; ** p < 0.01; * p < 0.05

 
