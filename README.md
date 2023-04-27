# Project_1
![alt text](https://learn.g2.com/hubfs/shopper%20marketing.jpg)

# Data Science and Grocery Sales
## Analyzing Outlet Sales  

**Eli Spreng**: 

### Business problem:

In looking at grocery sales, interested parties want to know what will will increase sales. This project analyzes what factors have the greatest impact on 
grocery outlet sales.


### Data:
Big Market Sales Prediction: https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/#About 

#### Visual 1: Bar Graph Showing Top 15 Coefficients for Linear Regression
![alt text](https://github.com/Elispreng/Project_1/blob/main/Images/Top%2015%20with%20Linear%20Regression2.png)

#### Interpretation of Coefficients
- Item Type Seafood: Seafood sales affect sales more
- Outlet Type Supermarket: Supermarkets sell more than grocery.
- Item Type Starchy Foods: Starchy foods affect sales. 
- Item Type Breads: Breads sell more
- Outlet Locaion:  where the supermarket is  affects sales. 


#### Visual 2: Bar Graph Showing Top  Features for Random Forest
![alt text](https://github.com/Elispreng/Project_1/blob/main/Images/Feature%20Importance%20for%20Random%20Forest.png)

#### Interpretation  of Top 5 Features for Random Forest
- Item MRP: suggest retail prices affects the sale
- Item visibility affects the sales
- Item weight affects the sales
- Outlet Year affects the sales: when the outlet was built. 
- Snack Foods affect the sales

#### Visual 3: Bar Graph Showing Top 15 with Shap
![alt text](https://github.com/Elispreng/Project_1/blob/main/Images/Shap%20Bar%20Plot.png)

### Feature Comparison
-The feature comparisons with Shap are  almost the same. The only difference is the fifth feature. In  Shap, it is Outlet type and and in the original random forest  the fifth feature was snack foods. 

#### Visual 4: Shap Summary Dot Plot
![alt text](https://github.com/Elispreng/Project_1/blob/main/Images/Shap%20Summary%20Plot2.png)

Three most important features interpretation:
Item MRP: lower the MRP the more likely the model will predict a sales price.
Item Visibility: Higher value of Visibility leads to lower sales.
Item Weight: Higher value of Weight leads to lower sales.

### First Example:High Visibility
#### Interpretation of LIME
![alt text](https://github.com/Elispreng/Project_1/blob/main/Images/HighVizLIME.png)
The predicted sales value is 369.03
Orange signifies the positive impact and blue signifies the negative impact of that feature on the target. 
- Top 3 Positive impact on sales prediction 
  - item type of meat, supermarket type 2, location/tier 3 and frozen foods. 
- Top 3 Negative impact on sales prediction
 -  Item MRP, Breakfast, Snack Foods 

### Interpretation of Force Plot
![alt text](https://github.com/Elispreng/Project_1/blob/main/Images/HighVizForcePlot.png)
- In this case, item type meat has  a positive impact on the prediction. Outlet size medium and supermarket type 2 also have positive impact on predicting sales. Two  features  have a negative impact on the prediction. These features Item MRP and  visibility. 


### Second Example High MRP 
#### Interpretation of LIME
#### The predicted sales value is 260.93
  - Orange signifies the positive impact and blue signifies the negative impact of that feature on the target.
 - Positive impact on sales prediction
Item MRP, Item Visibillity, and Supermarket type 2
 - Negative impact on sales prediction
Starchy Foods, Hard Drinks, and Baking Goods

![alt text](https://github.com/Elispreng/Project_1/blob/main/Images/LIME_HighMRP2.png)

#### Interpretation of Forceplot 
In this case, feature 'Item MRP' and 'Outlet Size small' have a positive impact on the prediction, while 'Item Weight' and 'Item Visibility' have a negative impact on the prediction.
![alt text](https://github.com/Elispreng/Project_1/blob/main/Images/Force_Plot_High_MRP)
