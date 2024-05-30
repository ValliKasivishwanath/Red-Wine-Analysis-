# Red-Wine-Analysis-


**Abstract**

The Wine Quality dataset stands as a valuable resource in the realms of oenology and data science, offering a comprehensive exploration of the interplay between chemical components and sensory evaluations in red wines.This report investigates the determinants of red wine quality, employing a dataset with 1600 observations and 12 variables, including 11 independent factors (e.g., acidity, sulfur levels, alcohol percentage) and a dependent variable quality score (0-10).This is done to understand how specific chemical attributes are correlated with the perceived quality of wines. The findings offer insights crucial for producers seeking premium pricing and reputation-building, as well as enhancing consumer experiences. This analysis contributes to the economic, social, and cultural dimensions of the wine industry, fostering regional branding and consumer trust.

**Introduction**

**Importance:** Understanding red wine quality isn’t just about taste; it’s a blend of tradition, commerce, and cultural significance. For producers, it’s the key to setting premium prices and building a stellar reputation. For consumers, it ensures a delightful drinking experience. This study bridges the gap between the business of wine making and the cherished cultural traditions associated with it.

**Literature Review:** While previous research has touched on factors like acidity and sugar content, our study extends beyond, utilizing a rich dataset of 1600 observations and 12 variables. We aim to contribute to the existing knowledge by employing advanced statistical methods to unravel the specific chemical components influencing red wine quality.

**Summary of Findings:** In a nutshell, our analysis seeks to uncover the secrets behind red wine quality. The results promise valuable insights for producers and consumers alike, enhancing economic, social, and cultural dimensions within the wine industry. The interplay of tradition, science, and statistical analysis forms the core of our exploration, enriching the understanding of what truly makes red wine exceptional.

**QUESTION AND ASSOCIATED HYPOTHESIS**

**Question of Interest:** What chemical components significantly affect the quality of red wine?

**HYPOTHESIS FOR THE STUDY**

**NULL HYPOTHESIS (H₀):** No chemical components (independent variables) have significant impact on the quality score of red wines. B1 = 0

**ALTERNATIVE HYPOTHESIS (H₁):** There is a significant relationship between the chemical components and the quality score of red wines, indicating specific attributes influence perceived quality. B1 ≠ 0

**Independent Variable :** There are 11 Independent variables like fixed acidity,volatile acidity, citric acid, sugar content, chlorides, free sulfur dioxide, total sulfur dioxide, density,pH, sulfates,alcohol percentage.

**Dependent Variable:** Quality ( score between 0 and 10)

**Data Source:** https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009/code


Descriptive Statistics of Red Wine Quality
================================================
Statistic              N   Mean  Median St. Dev.
------------------------------------------------
alcohol              1,599 10.42 10.20    1.07  
volatile.acidity     1,599 0.53   0.52    0.18  
pH                   1,599 3.31   3.31    0.15  
sulphates            1,599 0.66   0.62    0.17  
residual.sugar       1,599 2.54   2.20    1.41  
total.sulfur.dioxide 1,599 46.47 38.00   32.90  
fixed.acidity        1,599 8.32   7.90    1.74  
citric.acid          1,599 0.27   0.26    0.19  
chlorides            1,599 0.09   0.08    0.05  
free.sulfur.dioxide  1,599 15.87 14.00   10.46  
density              1,599 1.00   1.00   0.002  
------------------------------------------------
**Mean and Standard Deviation**

**Alcohol (Mean: 10.42, St. Dev.: 1.07):** Average alcohol content is 10.42%, with a typical variation of ±1.07%. This indicates a moderate level of alcohol concentration common in red wines.

**Volatile Acidity (Mean: 0.53, St. Dev.: 0.18):** Average volatile acidity is 0.53 with a relatively narrow range of variation. Volatile acidity affects the aroma and taste of wine.

**pH (Mean: 3.31, St. Dev.: 0.15):** Average pH value is 3.31, indicating a typical acidity level for red wines. The low standard deviation shows that pH levels are quite consistent across the samples.

**Sulphates(Mean: 0.66, St. Dev.: 0.17):** Average sulphates content is 0.66, with a moderate range of variation. Sulphates can influence both the taste and preservation of wine.

**Residual Sugar (Mean: 2.54, St. Dev.: 1.41):** The mean residual sugar is relatively low at 2.54, but with a larger standard deviation, indicating more variability in sugar content among these wines.

**Total Sulfur Dioxide (Mean: 46.47, St. Dev.: 32.90):** Shows a high level of variation in total sulfur dioxide, which is used as a preservative in wine. The high standard deviation indicates diverse preservation levels.

**Fixed Acidity(Mean: 8.32, St. Dev.: 1.74):** Average fixed acidity is 8.32, with a fairly wide range of variation. Fixed acidity contributes to the tartness and sharpness of the wine.

**Citric Acid (Mean: 0.27, St. Dev.: 0.19):** Average citric acid content is relatively low, and its standard deviation suggests that the citric acid content varies among different wines. Citric acid can add freshness and flavor.

**Chlorides(Mean: 0.09, St. Dev.: 0.05):** The average chlorides level is low, indicative of the salt content in wine. The standard deviation is also low, showing less variation in saltiness.

**Free Sulfur Dioxide (Mean: 15.87, St. Dev.: 10.46):** Indicates a wide range of free sulfur dioxide content, which can affect both the taste and aroma of the wine.

**Density (Mean: 1.00, St. Dev.: 0.002):** The mean density is around 1.00, typical for wine, with a very low standard deviation, showing that density is quite consistent across different wine samples.

**HISTOGRAM OF ALCOHOL AND QUALITY** 

Observation from Histogram: The distribution of alcohol content appears to be right-skewed.

Implication: Most of the wines have a moderate alcohol content, with fewer wines having very high alcohol levels. Right skewness means the tail on the right side of the distribution is longer or fatter than the left side. In a positively skewed distribution, the mean is typically greater than the median.

**SCATTERPLOT FOR ALCOHOL VS QUALITY**

Positive Correlation: The upward-sloping trend line suggests a positive correlation between alcohol content and wine quality. This implies that, on average, wines with higher alcohol content tend to receive higher quality ratings.

Dense Population Between 9% to 12% Alcohol: The concentration of data points between 9% to 12% alcohol content indicates that the majority of sampled wines fall within this alcohol percentage range.

Spread of Points Around the Trend Line: The dispersion or spread of data points around the trend line suggests that, while alcohol content is correlated with quality, it is not the sole determinant. The variability in quality ratings at similar alcohol levels indicates the presence of other influential factors.

Recommendation for Further Statistical Analysis: Given the complexity of factors influencing wine quality, it is advisable to conduct additional statistical analyses. Regression analysis can help unravel the nuanced relationships between various independent variables (e.g., acidity, sulfates, residual sugar) and the dependent variable (quality). This deeper analysis can provide a more comprehensive understanding of the multifaceted nature of wine quality determination.

Outliers In our analysis, we observed that the dataset exhibits minimal instances of outliers.This suggests a relatively homogenous distribution of values, contributing to the robustness of our dataset for further analysis.

**SCATTERPLOT FOR VOLATILE ACIDITY VS QUALITY** 

Negative Correlation: The scatter plot shows a negative correlation between volatile acidity and quality, indicated by the downward slope of the red line of best fit. As volatile acidity increases, quality ratings tend to decrease.

Variability of Data: There is considerable spread around the line of best fit, suggesting that volatile acidity is not the only factor affecting quality—other variables may also play a role.

OUTLIERS: There are very few points at the quality extremes (quality levels 3 and 8), which could be considered outliers simply due to their rarity in the dataset.

**SCATTERPLOT FOR SULPHATES VS QUALITY** 

POSITIVE CORRELATION: The red line indicates a positive correlation between sulphates and quality. As the sulphate level increases, the quality rating seems to increase as well. The line of best fit slopes upward across the chart, which suggests that wines with higher sulphate levels tend to have higher quality ratings.

SPREAD OF DATA: The data points are spread around the line of best fit, indicating variability in quality ratings at different sulphate levels. While there’s a general trend, there are still variations in quality that aren’t explained by sulphate levels alone.

OUTLIERS: There do not appear to be extreme outliers as in the previous chart. However, there are a few points at higher levels of sulphates (above 1.5) with quality ratings that deviate from the trend. Additionally, there are some data points with low sulphate levels but relatively high-quality ratings.

**BASE REGRESSION ANALYSIS ON QUALITY**


Regression Analysis: Effect of Variables on Quality
============================================================================
                                       Dependent variable:                  
                     -------------------------------------------------------
                                             quality                        
                       (1)     (2)     (3)     (4)     (5)     (6)     (7)  
----------------------------------------------------------------------------
alcohol               0.361   0.314   0.309   0.309   0.294   0.292   0.298 
                     (0.018) (0.018) (0.018) (0.018) (0.019) (0.019) (0.019)
                                                                            
volatile.acidity             -1.384  -1.221  -1.221  -1.199  -1.188  -1.129 
                             (0.110) (0.111) (0.111) (0.113) (0.114) (0.117)
                                                                            
sulphates                             0.679   0.679   0.713   0.712   0.677 
                                     (0.126) (0.126) (0.123) (0.123) (0.123)
                                                                            
residual.sugar                               -0.002   0.009   0.008   0.003 
                                             (0.014) (0.014) (0.014) (0.014)
                                                                            
total.sulfur.dioxide                                 -0.002  -0.003  -0.003 
                                                     (0.001) (0.001) (0.001)
                                                                            
free.sulfur.dioxide                                           0.004   0.004 
                                                             (0.002) (0.002)
                                                                            
fixed.acidity                                                         0.024 
                                                                     (0.012)
                                                                            
Constant              1.875   3.095   2.611   2.615   2.817   2.815   2.541 
                     (0.185) (0.212) (0.217) (0.222) (0.231) (0.232) (0.275)
                                                                            
----------------------------------------------------------------------------
Observations          1,599   1,599   1,599   1,599   1,599   1,599   1,599 
R2                    0.227   0.317   0.336   0.336   0.344   0.345   0.348 
Adjusted R2           0.226   0.316   0.335   0.334   0.342   0.343   0.345 
Residual Std. Error   0.710   0.668   0.659   0.659   0.655   0.655   0.654 
F Statistic          468.267 370.379 268.912 201.570 167.097 139.922 121.091
============================================================================
Note:                                                                     NA

Alcohol (Coefficient Range: 0.292 to 0.361): A one-unit increase in alcohol is associated with an increase of 0.298 in quality. Higher alcohol content is consistently associated with higher quality ratings. The effect size varies slightly but remains significant.T-value: 20.06, Highly statistically significant

Volatile Acidity (Coefficient Range: -1.384 to -1.129): A one-unit increase in volatile acidity is associated with a decrease of 1.129 in quality. Volatile acidity negatively affects wine quality. Higher levels of volatile acidity are associated with lower quality ratings. This effect is quite significant in magnitude, suggesting a strong influence on quality perception. T-value: -12.58, Highly statistically significant.

Sulfates (Coefficient Range: 0.677 to 0.713): A one-unit increase in sulphates is associated with an increase of 0.677 in quality.. Sulphates show a positive relationship with wine quality. This indicates that wines with higher sulphates content tend to be rated higher in quality. T-value: 5.39, Statistically significant.

Residual Sugar (Coefficient Range: -0.002 to 0.009): A one-unit increase in residual sugar is associated with an increase of 0.003 in quality.The impact of residual sugar on quality is minimal and inconsistent across models, indicated by the small coefficients. This suggests residual sugar is not a strong predictor of quality in this dataset. T-value: -0.14, Not statistically significant (far below the threshold of 2 in absolute value).

Total Sulfur Dioxide (Coefficient Range: -0.003 to -0.002):A one-unit increase in total sulfur dioxide is associated with a decrease of 0.003 in quality. Total sulfur dioxide has a very small negative impact on quality. However, the effect is minimal, as indicated by the small coefficients. T-value: -2.00, Marginally statistically significant (on the threshold).

Free Sulfur Dioxide (Coefficient: 0.004): A one-unit increase in free sulfur dioxide is associated with an increase of 0.004 in quality. The effect of free sulfur dioxide on quality is positive but small, suggesting a limited impact.T-value: 2.00 , Marginally statistically significant (on the threshold).

Fixed Acidity (Coefficient: 0.024):A one-unit increase in fixed acidity is associated with an increase of 0.024 in quality. Fixed acidity shows a small positive relationship with quality in the final models, but again, the impact is relatively minor. T-value: 0.10, Not statistically significant.

Model Fit (R² Range: 0.227 to 0.348):The R² values, which measure the proportion of variance in quality explained by the models, improve as more variables are added. However, even in the most complex model (model 8), only about 34.8% of the variance in quality is explained, indicating that other factors not included in the model also play a significant role in determining wine quality.

Residual Standard Error: The residual standard error decreases as more variables are added, indicating a better fit of the model to the data.

In summary, the regression analysis suggests that alcohol content and volatile acidity are strong predictors of red wine quality, with alcohol positively associated and volatile acidity negatively associated with quality.

**ECONOMICAL SIGNIFICANCE**

Economic significance refers to the practical importance of the coefficients in real-world contexts, such as their impact on quality:

Alcohol: A positive and relatively large coefficient across all models suggests that alcohol content has a noticeable positive impact on quality.

Volatile Acidity: The negative coefficients indicate that higher volatile acidity reduces quality, and the magnitude suggests a substantial impact.

Sulphates: Positive coefficients with moderate size suggest a meaningful positive impact on quality.

Residual Sugar and Total Sulfur Dioxide: Small coefficients suggest these factors might have a limited economic impact on quality.

Free Sulfur Dioxide: Although statistically significant, the small coefficient indicates a limited practical impact.

Fixed Acidity: Given its small coefficient and high standard error, fixed acidity likely has minimal economic significance.

**LINEAR HYPOTHESIS TEST**

  Linear hypothesis test
  
  Hypothesis:
  sulphates = 0
  fixed.acidity = 0
  
  Model 1: restricted model
  Model 2: quality ~ alcohol + volatile.acidity + sulphates + residual.sugar + 
      total.sulfur.dioxide + free.sulfur.dioxide + fixed.acidity
  
  Note: Coefficient covariance matrix supplied.
  
    Res.Df Df      F    Pr(>F)    
  1   1593                        
  2   1591  2 19.045 6.704e-09 ***
  ---
  Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
F-Statistic (F): 19.045: This is the value of the F-statistic for the test. Model 2 provides a significantly better fit to the data than the restricted model (Model 1).

-The linear hypothesis test compares two models to assess the significance of sulphates and fixed acidity in predicting wine quality. The test reveals that including these variables significantly improves the model’s accuracy. The very low p-value (6.704e-09) strongly suggests that both sulphates and fixed acidity are key predictors of wine quality, rejecting the hypothesis that their coefficients are zero.

**Regression 7 was selected as the baseline model**

In selecting Regression 7 as the baseline model, we aimed to capture the fundamental factors influencing red wine quality. This model incorporates a well-rounded set of variables, including alcohol content, volatile acidity, sulphates, residual sugar, total sulfur dioxide, free sulfur dioxide, and fixed acidity.While Regression 7 includes multiple variables, it strikes a balance between complexity and interpretability. It is complex enough to capture the interplay of various factors affecting quality, yet not overly intricate to hinder practical application and understanding.By establishing this foundational model, we provide a comprehensive starting point for our analysis, ensuring that key components are considered before introducing the alternative regression analysis.

Overall, Regression 7 serves as a meaningful starting point, allowing for a comprehensive exploration of the relationships between key wine characteristics and quality.

**ALTERNATIVE REGRESSION ANALYSIS**


Regression Analysis: Interaction Model of Alcohol and sulphates
=========================================
                     Dependent variable: 
                     --------------------
                           quality       
                        (1)        (2)   
-----------------------------------------
alcohol                0.298     -0.082  
                      (0.019)    (0.079) 
                                         
volatile.acidity       -1.129    -1.100  
                      (0.117)    (0.116) 
                                         
sulphates              0.677     -4.979  
                      (0.123)    (1.214) 
                                         
residual.sugar         0.003      0.005  
                      (0.014)    (0.014) 
                                         
total.sulfur.dioxide   -0.003    -0.003  
                      (0.001)    (0.001) 
                                         
free.sulfur.dioxide    0.004      0.004  
                      (0.002)    (0.002) 
                                         
fixed.acidity          0.024      0.019  
                      (0.012)    (0.012) 
                                         
alcohol:sulphates                 0.562  
                                 (0.119) 
                                         
Constant               2.541      6.395  
                      (0.275)    (0.808) 
                                         
-----------------------------------------
Observations           1,599      1,599  
R2                     0.348      0.360  
Adjusted R2            0.345      0.357  
Residual Std. Error    0.654      0.648  
F Statistic           121.091    111.806 
=========================================
Note:                                  NA
Interpretation of Coefficients

Model (1) Alcohol (0.298): For every one-unit increase in alcohol, quality increases by 0.298 units, assuming all other variables are held constant.

Volatile Acidity (-1.129): For every one-unit increase in volatile acidity, quality decreases by 1.129 units, holding other factors constant.

Sulphates (0.677): Each one-unit increase in sulphates is associated with an increase of 0.677 units in quality, with other variables constant.

Residual Sugar (0.003): A one-unit increase in residual sugar increases the quality by 0.003 units, all else being equal.

Total Sulfur Dioxide (-0.003): With each unit increase in total sulfur dioxide, there’s a decrease of 0.003 units in quality, assuming other factors remain constant.

Free Sulfur Dioxide (0.004): For every one-unit increase in free sulfur dioxide, quality increases by 0.004 units, other variables held constant.

Fixed Acidity (0.024): Each one-unit increase in fixed acidity results in an increase of 0.024 units in quality, keeping other factors the same.

Model (2)

Alcohol (-0.082): For each one-unit increase in alcohol, quality decreases by 0.082 units, assuming other variables are constant. This is a change from Model (1), likely due to the interaction with sulphates.

Volatile Acidity (-1.100): A one-unit increase in volatile acidity decreases the quality by 1.100 units, with all other variables held constant.

Sulphates (-4.979): Each one-unit increase in sulphates decreases the quality by 4.979 units, assuming other factors remain constant. This dramatic change from Model (1) is due to the interaction term.

Residual Sugar (0.005): A one-unit increase in residual sugar is associated with an increase of 0.005 units in quality, other factors being equal.

Total Sulfur Dioxide (-0.003): For each unit increase in total sulfur dioxide, there’s a decrease of 0.003 units in quality, keeping other variables constant.

Free Sulfur Dioxide (0.004): Each one-unit increase in free sulfur dioxide increases quality by 0.004 units, with other factors held constant.

Fixed Acidity (0.019): A one-unit increase in fixed acidity leads to an increase of 0.019 units in quality, assuming no changes in other variables.

Alcohol:Sulphates (0.562): This interaction term implies that the impact of alcohol on quality increases by 0.562 units for each one-unit increase in sulphates, and vice versa. This term indicates that the effect of each on quality is not independent but interdependent.

CONSTANT (INTERCEPT): This represents the expected value of the dependent variable when all independent variables are zero.

**STATISTICAL SIGNIFICANCE:**

The coefficients for alcohol, volatile.acidity, and sulphates are statistically significant in Model (1), as indicated by their standard errors which are relatively small compared to the coefficients themselves. In Model (2), the introduction of the interaction term alcohol:sulphates changes the significance of the alcohol and sulphates coefficients. The interaction term itself has a coefficient of 0.562 with a standard error of 0.119, indicating statistical significance. The F statistics for both models are high, which suggests that the variables, as a set, are statistically significant predictors of wine quality. The p-values associated with these coefficients (not provided here) would typically need to be below a threshold (such as 0.05) to be considered statistically significant.

OBSERVATIONS: The number of data points used in the analysis is 1,599 for both models.

R2 and ADJUSTED R2: These are measures of the model’s goodness of fit. R2 of 0.348 in model (1) and 0.360 in model (2) suggests that approximately 34.8% and 36.0% of the variability in quality is explained by the model, respectively. Adjusted R2 adjusts for the number of predictors in the model, providing a more accurate measure in the presence of multiple variables.

RESIDUAL STANDARD ERROR: This shows the average amount that the response will deviate from the true regression line.

**KEY INSIGHTS**

-The inclusion of the interaction term significantly changes the interpretation. While alcohol and sulphates individually seem to have a negative effect on quality in Model 2, their combined presence actually improves quality. -The interaction term suggests a synergistic effect: the presence of both high alcohol and high sulphates works better for quality than each component separately. -The R2 value in Model 2 (0.360) is slightly higher than in Model 1 (0.348), indicating a better fit to the data when the interaction term is included. -In summary, the analysis underscores the importance of considering interaction effects in regression models, as they can reveal complex relationships between variables that are not apparent when variables are considered individually.

**Linear hypothesis test**

Hypothesis:
alcohol:sulphates = 0

Model 1: restricted model
Model 2: quality ~ alcohol + volatile.acidity + sulphates + residual.sugar + 
    total.sulfur.dioxide + free.sulfur.dioxide + fixed.acidity + 
    alcohol:sulphates

Note: Coefficient covariance matrix supplied.

  Res.Df Df      F    Pr(>F)    
1   1591                        
2   1590  1 22.117 2.787e-06 ***
---
Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
Hypothesis interaction term

Model 1 (Restricted Model): Does not include the interaction term between alcohol and sulphates. Model 2 (Full Model): Includes the interaction term along with other predictors. **Key Results*: Residual Degrees of Freedom (Res.Df): Model 1: 1591 Model 2: 1590 The decrease by one degree of freedom in Model 2 indicates the addition of the interaction term.

Difference in Degrees of Freedom (Df): The difference of 1 degree of freedom reflects the inclusion of the interaction term in Model 2. F-Statistic (F): 22.117: This is a measure of the change in the model’s explanatory power due to the addition of the interaction term. The value of 22.117 is relatively high, indicating a significant effect of including the interaction term.

P-Value (Pr(>F)): 2.787e-06: -The p-value is extremely small (2.787e-06), indicating a highly significant effect of the interaction term. It strongly suggests that the interaction between alcohol and sulphates is a significant predictor of wine quality.

-The linear hypothesis test results show that the interaction term alcohol:sulphates significantly improves the model’s ability to predict wine quality. The inclusion of this term captures a synergistic effect that is not evident when considering alcohol and sulphates individually. This suggests that the combined effect of alcohol and sulphates on wine quality is substantial and important to consider in the model.

**Internal Validity Threats:**

Selection Bias in Data Collection: The dataset may primarily include wines from a certain price range or from prestigious vineyards, it may not accurately represent the full diversity of wines available in the market. Confounding Variables: Factors like vineyard location or grape variety, if not included, could confound the relationship between the variables (like alcohol content, acidity) and wine quality.

**External Validity Threats:**

Different Conditions: The effect of variables like alcohol content on wine quality could vary under different production methods, storage conditions, or consumer preferences, Climate conditions can alter the relationship. Measurement Error: For example, if the quality of wine is not measured consistently, or if there is error in measuring variables like alcohol or sulphate content, it can lead to incorrect conclusions about their effects.

**CONCLUSION**

-The introduction of the interaction term between ‘alcohol’ and ‘sulphates’ in Model 2 significantly changes the influence of these individual factors on quality, this makes ‘alcohol’ and ‘sulphates’ individually less influential while their interaction is positively significant.

-Most variables are statistically significant predictors of wine quality, with ‘alcohol:sulphates’ having a positive effect, suggesting a combined impact on quality.

-Chemical components significantly affect the quality of red wine are alcohol, sulphates and volatile acidity
