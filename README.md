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
![alt text] (https://github.com/Elispreng/Project_1/blob/main/Images/Shap%20Bar%20Plot.png)

### Feature Comparison
-The feature comparisons with Shap are  almost the same. The only difference is the fifth feature. In  Shap, it is Outlet type and and in the original random forest  the fifth feature was snack foods. 

#### Visual 4: Shap Summary Dot Plot
![alt text] (https://github.com/Elispreng/Project_1/blob/main/Images/Shap%20Summary%20Plot2.png)

Three most important features interpretation:
Item MRP: lower the MRP the more likely the model will predict a sales price.
Item Visibility: Higher value of Visibility leads to lower sales.
Item Weight: Higher value of Weight leads to lower sales.

### Cannot save images
#### Interpretation of LIME
The predicted sales value is 369.03, Orange signifies the positive impact and blue signifies the negative impact of that feature on the target. The positive impact on sales prediction are item type of meat, supermarket type 2, location/tier 3, and item weight. Item_MRP, hard drinks, Breakfast, canned, fruits/vegetables, and health/hygiene have negative impact on sales prediction

### Cannot add Forceplot image
In this case, outlet type supermarket 1 and 2 have a positive impact on the prediction. The third factor of weight also has positive impact on predicting sales. Many features have a negative impact on the prediction. These features Item MRP, visibility, and the size of the outlet as small.
