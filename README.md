# 1. Introduction
In recent years, the tourism industry has gained a good market. Especially with the growth in e-commerce development, selecting overseas destinations has become easier over the Internet. Moreover, for most people, choosing the best hotel is considered an important part of a good trip.

It might be challenging to choose which among the hundreds or even thousands of hotels available at a given location will best fit your needs. By offering consumers individualized hotel recommendations, most travel companies hope to pull users out of the classic rabbit hole associated with hotel searches.

Expedia wants to take the proverbial rabbit hole out of hotel search by providing personalized hotel recommendations to their users. This is no small task for a site with hundreds of millions of visitors every month. Expedia uses search parameters to adjust their hotel recommendations, but there isn't enough customer-specific data to personalize them for each user.

Expedia provided a data set that captured the logs of user behaviour. These include details about what the customers searched for, and how they interacted with the search results - i.e. whether they actually booked the hotel or simply clicked to view details, whether or not the search result was a travel package, and so on. 

# 1.1 Problem statement

Organizing your ideal gateway, whether it's a dream holiday or a brief weekend retreat, can often feel daunting. With a seemingly endless array of hotels at each destination, selecting the perfect one that aligns with your tastes can be challenging. 

Do you opt for a familiar favorite with those delightful pillow mints, or venture into something new with a chic pool bar? The idea of vacation is leisure and thus providing personalized hotel recommendations can be ease to the user. Providing a better user experience, increasing customer satisfaction, and improving the overall revenue of the hotel industry. Expedia wants to contextualize customer data and predict the likelihood a user will stay at 100 different hotel groups.

# 1.2 Objective

The primary goal is to predict which “hotel cluster” the user is likely to book, given his search details. These “clusters” have been created by Expedia based on some undisclosed in-house algorithms. But the intuition is that hotels belonging to a cluster are similar for a particular search - based on historical price, customer star ratings, geographical locations relative to city center, etc. These hotel clusters serve as good identifiers to which types of hotels people are going to book, while avoiding outliers such as new hotels that don't have historical data. The goal will enhance the user experience on Expedia's platform, making hotel selection a seamless, intuitive, and highly personalized process. 
And the next goal is to explore and evaluate the performance of multiple classification algorithms and select the best-performing model based on an evaluation metric.

# 2. Dataset

# 3. Framework

![image](https://github.com/user-attachments/assets/f266ba67-a4a6-461f-b3fb-e93bcac2e4f5)

Fig 1. Framework

In the data acquisition stage, the dataset is we downloaded from the source i.e Kaggle site. Then in the data preprocessing step, the size of the data is we down sample and also checked for missing values also. In the next stage, feature engineering is performed where  new features are generated from the original feature. Moreover, PCA dimensionality reduction method is employed for the destination dataset. The model implementation was done using Random forests, Logistic regression, k-Nearest neighbours and Decision tree.

# 4. Methodology 

The implementation was done using Jupyter notebook and libraries such as pandas, numpy, matplotlib, seaborn, scit-learn were used.

The implementation is shown the following steps: 

- First, the train data will be processed and modeled using machine learning algorithms, and accuracy will be assessed.
- Second, the destinations data will be explored, merged with the train data, and modeled using the same machine learning algorithms. Accuracy will also be evaluated.
- Third, the algorithm achieving the higher accuracy will be selected for further evaluation. The model's ability to predict the true label within its top 5 predictions will be assessed.


