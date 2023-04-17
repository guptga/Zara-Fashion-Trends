# Zara Fashion Trends

The main goal if this project is to use sales data from previous weeks to predict best perfomring products.

## Components:

### EDA, Data Transformation and Feature Engineering 

** Data Transformation **
After EDA, the following aggregation results were added into the original data for additional features:
1. As multpile products can belong to a certain block, a num_items column was added
2. Because we are most concerned with data at a product level color_id and sales_id columns were removed
3. For the added clusters column, the last day in training data (day 84) was used in the following unsupervised ML: k-means (to find the optimal number of clusters) and PCA (to reduce the dimenstion and give us cleaner clusters)[^1]
4. A new dataframe was created including the above mentioned columns for the model training.

**Feature Engineering**
*Model Training*




[^1]: Interestingly, this new feature ended up being second important feature in the last (or best) model.
