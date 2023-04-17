# Team 10- Zara Fashion trends



![image](https://cloudinary.hbs.edu/hbsit/image/upload/s--YocdHEbD--/f_auto,c_fill,h_375,w_750,/v20200101/A17A58369E0D9FBC28574F424FBDB551.jpg)

## Team Members: 
Elsa Figueroa

Gauri Gupta

Miga Budaasuren

Termeh Mohebbie

  

# Introduction											
Predictive analytics is an advanced analytics method that leverages historical data, statistical modeling, data mining, and machine learning techniques to predict future outcomes. Companies use predictive analytics to identify risks and opportunities by finding patterns in data. Predictive analytics is associated with big data and data science. Data scientists use machine learning algorithms such as deep learning, logistic and linear regression models, neural networks, and decision trees to make predictions and gain insights from data. These modeling techniques can build on initial predictive insights to make additional predictions.



### Dataset: 



### Goal: The main goal is to predict best-performing products for the last week in terms of revenue using the previous weeks data


# ETL				


#### Cleaning 							



#### Feature Selection

***Correlation Matrix with Heatmap*** - Correlation is a measure of how features are related to each other or the target variable, and can be positive or negative. Positive correlation means an increase in one feature value leads to an increase in the target variable value, while negative correlation means an increase in one feature value leads to a decrease in the target variable value. To identify which features are most related to the target variable, a heatmap of correlated features can be plotted using the Seaborn library. The heatmap makes it easy to visualize the degree of correlation between different features and the target variable.

![image](https://user-images.githubusercontent.com/116124534/232615274-3d7a400d-6986-4e93-9d5b-4c775a4dca63.png)


# Machine Learning


***StandardScaler*** is a fast and specialized algorithm for scaling data. It calculates the mean and standard deviation of the data set and normalizes it by subtracting the mean and dividing by standard deviation. Using StandardScaler is a common practice in ML projects if the data set follows a normal distribution.  


We initiated our machine learning successfully with XG Boost, Random forest and failed models with Logistic Regression and Gausian NB

***Logistic Regression***: The Logistic Regression model is based on the logistic function, which maps any real-valued input to a probability value between 0 and 1. The logistic function is a type of sigmoid function, which has an S-shaped curve. The logistic regression model fits the sigmoid function to the input data and finds the coefficients that maximize the likelihood of the observed outcomes.

***Gaussian Naive Bayes***: Gaussian Naive Bayes (NB) is a probabilistic machine learning algorithm used for classification problems. It is based on Bayes' theorem and assumes that the features are independent of each other given the class.The Gaussian NB model assumes that the continuous features of the dataset follow a Gaussian (normal) distribution, while the categorical features follow a multinomial distribution. This means that the model calculates the mean and variance of each continuous feature for each class and uses them to calculate the probability of a new data point belonging to each class.

***Decision Tree***: A decision tree can be used to visually and explicitly represent decisions and decision making. As the name goes, it uses a tree-like model of decisions. It makes predictions based on how a previous set of questions were answered.



***Random Forest***: Random Forest is a popular supervised machine learning algorithm used for classification and regression problems. It builds decision trees on different samples and takes their majority vote for classification or average for regression. Random Forest can handle data sets containing continuous and categorical variables. It performs well for classification and regression tasks and is widely used by data scientists.


***XGBoost***:XGBoost is an extension of the Gradient Boosting algorithm, which trains models sequentially to correct the errors of the previous models. However, XGBoost includes additional features that make it more efficient and effective than traditional Gradient Boosting, such as regularization to prevent overfitting and handling missing values.




