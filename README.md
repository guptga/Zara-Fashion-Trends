# Zara Fashion Trends

The main goal if this project is to use sales data from previous weeks to predict best perfomring products.

## Components:

### Data Transformation, EDA and Feature Engineering 

** EDA **

We first summarize data 
![image](https://user-images.githubusercontent.com/116039323/232681011-73c66132-cd58-4995-ad99-3affcd1f5630.png)

We made a line chart to display the trend of sales over weeks
![image](https://user-images.githubusercontent.com/116039323/232681316-5907b2be-1857-40ab-83de-b0c635afcf86.png)

A correlation heat map was created to determine correlation strengths between columns
![image](https://user-images.githubusercontent.com/116039323/232681542-bdeb8381-ba40-40b7-8c1e-1ae13d3a821c.png)

We created pie charts for color and stock number organizzed by price
![image](https://user-images.githubusercontent.com/116039323/232681728-b3190ba6-727b-4d9a-a091-e048de7d831d.png)


** Data Transformation **

Raw data was in 4 csvs

First thing done was organize the positions data and add cols pos_count, pos_min (the min amount of times item occurs on a certian day), pos_max (same as above but max), pos_mean

Next, we move to the blocks data where first of all we sort the data and add col num_itmes counting the number of items in each particular block

For the sales_stock we remove color andsize as it is not relevant for the scope of our project but we did keep it for our EDA as we thought it was intersting information that maybe could be explored further in the future. we then aggregate by product_id

We then merged all the transformed data 

With this dataframe we cluster day 84 weuse cols product_id num_items stock price and pos_ count and drop non-numerical values, normalize the data with scaler

determined was the optimal number of clusters is 4 and we plot these clusters, we then merge the cluster data with the final dataframe we created earlier withthe transformed data


**Feature Engineering**

ML models used are RF, XG Boost and DL

Below are the experiment results:
![Screenshot (9)](https://user-images.githubusercontent.com/116039323/232682613-0e9deae3-0971-4c78-baa9-a54203ca2468.png)

We then made a relevance bar chart 
![image](https://user-images.githubusercontent.com/116039323/232682917-b27dffef-54e3-4651-aad1-9bf97aaf3ddf.png)

Here are our predoctibility accuracy rates
![Screenshot (11)](https://user-images.githubusercontent.com/116039323/232683161-fa908d4a-c2f5-49f0-85d8-6f65b5d451e7.png)
There is absolutely room to improve but we are happy with these results





[^1]: Interestingly, this new feature ended up being second important feature in the last (or best) model.


