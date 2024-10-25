# JewelryOptimizer

## Project Background

Gemineye Emporium is a jewelry provider operating in the jewelry market. They expanded from a relatively small-scale jewelry provider to a large-scale jewelry designing and trading company. Although this transition has gone well, it has not gone without some issues that the company board did not see coming. These edge cases were further looked into and a particular one is with the prices of products. 

Insights and recommendations are provided on the following key areas:

- **Category 1:** Types of Jewelry presently being sold
- **Category 2:** The gender of their customers catered for most in each of those categories 

The code used for data preparation can be found here [link](https://github.com/Three2Two/JewelryOptimizer/blob/main/Jewelry_optimizer.ipynb#eda).

Pipelines built for various model creations can be found here [link](https://github.com/Three2Two/JewelryOptimizer/blob/main/Jewelry_optimizer.ipynb#data-modelling).

Evaluation of the various models can be found here [link](https://github.com/Three2Two/JewelryOptimizer/blob/main/Jewelry_optimizer.ipynb#model-eveluation).



# Data Structure & Initial Checks

The company's main database structure as seen below consists of 2 tables: with a total row count of 95910 records. A description of each table is as follows:
- **Table 1:** Has 13 columns which include features such as ('Product_ID', 'SKU_Quantity', 'Category_ID', 'Category_alias', 'Brand_ID', 'Price_USD', 'User_ID','Product_gender','Main_color', 'Main_metal')
- **Table 2:** The description of each column 



# Executive Summary

### Overview of Findings

Our analysis of jewelry sales reveals that over 95% of purchases were made by female customers, with earrings and pendants contributing to more than 50% of total sales. These two categories are the most frequently sold items, indicating a strong preference in the market.

Despite the wealth of data, the predictive models developed to understand customer behavior and sales patterns performed poorly, with the best model achieving only a 32% prediction accuracy. This underperformance is primarily attributed to the nature of the available features and the high skewness in pricing data.

![Most sold jewelry items](https://github.com/Three2Two/JewelryOptimizer/blob/main/images/pendandear.png)
![Male and female customers](https://github.com/Three2Two/JewelryOptimizer/blob/main/images/malenfemale.png)



# Recommendations:

Based on the insights and findings above, we would recommend Gemineye Emporium stakeholders to consider the following: 

* More sales are being made to females than to males. **An ad campaign should be carried out to boost jewelry sales to more males.**
  
* Earrings and rings were the main items being sold. **Other items like pendants could be sold as a set with earrings and rings to increase sales.**
  
* **More features such as customer demographic and purchasing behavior should be added to ensure proper data integrity.**. This stems from the fact that the features present were not enough to build robust models with high predictive value. 
  


# Assumptions and Caveats:

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

* **Assumption 1:** Missing values in the data were replaced with the most frequent in each column.
  
* **Assumption 2:** Categories in the jewelry category columns had numerical values and these were dropped from the data and this led to the loss of over 10k rows of data. 
