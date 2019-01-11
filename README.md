# Statistical-Modeling-in-R
Stat-420 Course, Summer 2018

## About the project
There are many brew enthusiasts who like to brew beer at home. In order to make a good beer or to improve a recipe over many tries, it is essential to capture readings for several attributes during and after the brewing process. This requires one to buy costly sensors or measuring gadgets. Using Applied Statistics with R we wish to check if we can analyze and predict any of the attributes of beer, and hopefully suggest cost savings by eliminating any sensors or measuring gadgets for it. Further, we can even predict any attribute of the final product in the early stages of brewing process so that any tweaks can be made to the recipe based on the knowledge of the predictions of the final product.

## Methodology/Approach

We develop 3 studies/models and pick the best among them. Below is the approach: 

1) Split data into train and test set; 20% of randomly picked data shall be set asside as test data and remaining 80% as test data. Models will be fit using train data and their performance on test data shall be captured. Metrics captured on the test data will mainly decide the best model.
2) Fit different models using below approaches, 
 -- Use an additive model using all attributes as starting model and do backward search using AIC and BIC
 -- Use a model with all two-way interactions along with their main effects as starting model and do backward search using AIC
and BIC
 -- Use a model with two-degree polynomials for all attributes along with their main effects as starting model and do backward
search using AIC and BIC
3) For each model capture the metrics defined in next sub-section on train and test data.
4) We’ll then pick the best model based on metrics and further tune or diagnose it for leverages, outliers and influencial observations.
