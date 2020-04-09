# Market_Basket_Analysis

Understand patterns in orders placed on Instacart

## Team Members 

- Sahit Koganti (M13262499)
	
- Yashwanth Kumar Yelamanchili (M13437471)

## Data Source

- The Instacart Online Grocery Shopping Dataset 2017, Accessed from https://www.instacart.com/datasets/grocery-shopping-2017 on 04th April 2020

- Access the metadata from https://gist.github.com/jeremystan/c3b39d947d9b88b3ccff3147dbcf6c6b

## Process Flow

- Data Loading
- Data Cleaning
- EDA
- Modeling
- Summary

## Implementation Plan

### Data Extraction

- Web scraping technique has been implemented to fetch the data from the link mentioned above

- The technique also includes unzipping the data file and placing the individual datasets in the same folder where the code is located 

### Data Cleaning

- Data counts, missing values and unique values have been checked

- Missing values have been replaced with '999' for the column 'days_since_prior_order'

### Data Merging

- All the individual datasets have been merged to form a master dataset

- We will form smaller subsets from this master dataset for performing EDA

### EDA

- Orders count by the day of Week and Hour 

	- Top products by day of week 

	- Top products by hour 

- Orders count by departments 

	- Top products by department 

- Orders count by Aisles 

	- Top products by aisles 

- Order count in the Non-perishables products - filter departments/aisles 

- Recency - Frequency Analysis 

	- Grouping customer by recency 

- Add_to_cart_order 

	- Analyzing the rank in which products are added across baskets 