# Zara Fashion Trends


![image](https://cloudinary.hbs.edu/hbsit/image/upload/s--YocdHEbD--/f_auto,c_fill,h_375,w_750,/v20200101/A17A58369E0D9FBC28574F424FBDB551.jpg)


# Introduction											
Predictive analytics is an advanced analytics method that leverages historical data, statistical modeling, data mining, and machine learning techniques to predict future outcomes. Companies use predictive analytics to identify risks and opportunities by finding patterns in data. Predictive analytics is associated with big data and data science. Data scientists use machine learning algorithms such as deep learning, logistic and linear regression models, neural networks, and decision trees to make predictions and gain insights from data. These modeling techniques can build on initial predictive insights to make additional predictions.


## Objective: 

The main goal of this project is to use sales data from previous weeks to predict best performing products.

## Methodology


**EDA**<br>

We first summarize data <br>
![image](https://user-images.githubusercontent.com/116039323/232681011-73c66132-cd58-4995-ad99-3affcd1f5630.png)<br>

We made a line chart to display the trend of sales over weeks<br>
![image](https://user-images.githubusercontent.com/116039323/232681316-5907b2be-1857-40ab-83de-b0c635afcf86.png)<br>

A correlation heat map was created to determine correlation strengths between columns<br>
![image](https://user-images.githubusercontent.com/116039323/232681542-bdeb8381-ba40-40b7-8c1e-1ae13d3a821c.png)<br>

We created pie charts for color and stock numbers organized by price
![image](https://user-images.githubusercontent.com/116039323/232681728-b3190ba6-727b-4d9a-a091-e048de7d831d.png)


**Data Transformation**<br><br>

Raw data was in 4 csvs

1. First thing done was organize the positions data and add cols pos_count, pos_min (the min amount of times item occurs on a certian day), pos_max (same as above but max), pos_mean

2. Next, we move to the blocks data where first of all we sort the data and add col num_itmes counting the number of items in each particular block

3. For the sales_stock we remove color andsize as it is not relevant for the scope of our project but we did keep it for our EDA as we thought it was intersting information that maybe could be explored further in the future. we then aggregate by product_id

4. We then merged all the transformed data 

5. With this dataframe we cluster day 84 weuse cols product_id num_items stock price and pos_ count and drop non-numerical values, normalize the data with scaler

6. We determined was the optimal number of clusters is 4 and we plot these clusters, we then merge the cluster data with the final dataframe we created earlier withthe transformed data


**Feature Engineering**

ML models used are RF, XG Boost and DL

Below are the experiment results:

![Screenshot (9)](https://user-images.githubusercontent.com/116039323/232682613-0e9deae3-0971-4c78-baa9-a54203ca2468.png)

We then made a relevance bar chart 

![image](https://user-images.githubusercontent.com/116039323/232682917-b27dffef-54e3-4651-aad1-9bf97aaf3ddf.png)

Here are our predictability accuracy rates

![Screenshot (11)](https://user-images.githubusercontent.com/116039323/232683161-fa908d4a-c2f5-49f0-85d8-6f65b5d451e7.png)<br>


There is absolutely room to improve but we are happy with these results


## Team Members: 
Elsa Figueroa

Gauri Gupta

Miga Budaasuren

Termeh Mohebbie


[^1]: Interestingly, this new feature ended up being second important feature in the last (or best) model.


