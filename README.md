# Market Basket Analysis

Understand patterns in orders placed on Instacart

## Team Members 

- Sahit Koganti (M13262499)
	
- Yashwanth Kumar Yelamanchili (M13437471)

## Data Source

- The Instacart Online Grocery Shopping Dataset 2017, Accessed from https://www.instacart.com/datasets/grocery-shopping-2017 on 04th April 2020

- Access the metadata from https://gist.github.com/jeremystan/c3b39d947d9b88b3ccff3147dbcf6c6b

## Process Flow

- Introduction
- Data Loading and Cleaning
- Data Merging
- Data Exploration
- Data Modeling
- Conclusion

## Implementation Plan

### Packages Used

- matplotlib.pyplot
- seaborn
- pandas
- os
- numpy
- warnings
- collections
- itertools
- sklearn

### Data Loading and Cleaning

- Web scraping technique has been implemented to fetch the data from the link mentioned above

 - First we need to run the notebook "Data_Download_using_WebScraping" to download the data as a zipped folder and unzip the files
 - Then, we need to run the notebook "Market_Basket_Analysis" for the entire analysis 

- Aisle tagging was done manualy to identify preishable and non-perishable products. This new tagged file is uploaded onto Github and the new file is read into the notebook using the Github link

- Data counts, missing values and unique values have been checked

- Missing values have been replaced with '999' for the column 'days_since_prior_order'

### Data Merging

- All the individual datasets have been merged to form a master dataset

- We will form smaller subsets from this master dataset for performing EDA

### Data Exploration

- What time and day of the week are the customers placing the orders?

- What are the products which drive the orders i.e. products which make or break the order?

- What are the products that are being re-ordered?

- What percentage of products being ordered are perishables / non-perishables?

- What are the departments / aisles that have the most number of orders? and re-orders?

- Does the re-order ratio of products change by time or day of the week?

- Is there any relation between the order in which the products are added to the cart with the re-order of that product?

- How frequently does the customer place the order on the Instacart app?

- How many products does a customer generally buy in each order?

### Data Modeling

5 models have been implemented in this project

- Association Rules - This will help in product recommendations i.e. based on the historical trasactions, this will tell us what product could be suggested if 
the customer adds product A to his cart

- Principal Component Analysis - This will tell us how can we reduce the dimensionality of the dataset while retaining the percentage of variability being explained. This will 
feed in as an input into the clustering analysis where we decide on the number of clusters

- Customer Segmentation - We use k-means clustering to group customers into 5 clusters based on their ordering pattern from aisles

- Word2vec - This will help in calculating user similarity score based on the products purchased and the order in which the orders are purchased. Word2vec can be 
thought of as a two-layer neural net that processes text by “vectorizing” words. Its input is a text corpus and its output is a set of vectors: feature vectors that represent words in that corpus

- TF-IDF Transformation and Vectorization - This will also help in calculating user similarity score based on the products purchased and the order in which the 
orders are purchased. This principle is based on matrix decomposition


## References

The following notebooks and articles are used as references for implementing exploration and modeling techniques

- https://gist.github.com/jeremystan/c3b39d947d9b88b3ccff3147dbcf6c6b

- https://www.slideshare.net/dominodatalab/data-science-at-instacart-making-ondemand-profitable

- https://artindatascience.wordpress.com/instacart-kaggle-competition/

- https://www.kaggle.com/sudalairajkumar/simple-exploration-notebook-instacart 

- https://www.kaggle.com/omarito/word2vec-for-products-analysis-0-01-lb 

- https://www.kaggle.com/kashdotten/customer-segmentation-pca-elbow-k-means-apriori 

- https://www.kaggle.com/asindico/customer-segments-with-pca 

- https://www.kaggle.com/datatheque/association-rules-mining-market-basket-analysis 
