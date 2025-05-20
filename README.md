# Real-Estate-Predictor

## Introduction:

Our goal was to create a model that would assist homebuyers in filtering  properties based on feature importance. Due to data limitations, our driving factors were square footage and location (determined by city and/or neighborhood).  Additionally, our other model aims to identify which factors tend to have the highest effect on sale price. The ultimate goal of this project is to gain a better understanding of what drives sale price and then use that knowledge to help predict sale price. This system could be beneficial for home buyers interested in seeing what the driving factors are in a home’s listed price.

## Background:

In an evolving real estate market, it is important to have accurate property valuations for potential buyers and sellers. Not only is just critical for the buyers and sellers but it is also very important for economists and urban planners as well. Traditional appraisal methods, while effective, are often extremely time consuming and may not capture the entire complexity of real estate and how residential real estate is influenced by numerous factors ranging from physical attributes to different amenities. To bridge this gap we decided to try a machine learning approach in order to save time and make it easier for buyers, sellers, economists etc. 

An important aspect of this project to consider is the construction of an individual evaluation mechanism. After the construction of the first model to predict sale price, we developed a system to gain insight into the exact drivers of the price. This comprehensive analysis was gained through an analysis of feature importance through the Random Forest Regressor.

## Experimental Setup:

Datasets:
- Our datasets were found from Kaggle, searching for real estate data in different cities. It was difficult to find datasets that would work for our model, but we determined specific features that each dataset had, removed the other features, and combined them together. We split the dataset in half for training and testing. 

Model:
- For the price prediction model we used a Random Forest format based off of the user inputs. From our references, we found that Random Forest would be the best model for us to use as we were basing our model off of Alan Ihre’s paper and research.  The datasets used for this model were mainly focused on major cities throughout the United States. 

Evaluation Metrics:
- The evaluation metrics used for our model are $R^2$ and RMSE.

## Results:

Task One:
- The results were extremely strong with $R^2$ and RMSE at 0.73 and 684,889 respectively.
- As we continued to add datasets, our estimations became affected despite continued increases in R2 and decreases in RMSE. This was a result of increased information for locations contained across multiple datasets. 

Task Two: 
- The aim of task two was to figure out which features carry the most weight  when it comes to influencing sale price based on the available data. The graph below shows which features were determined  to be the most important, and in our case it was square footage which we predict would stay as the dominant factor if more features were added.

## Summary & Conclusion:
Task One:
- The first task of the model was not as good as it could have been because of the fact that we did not have all the data that we needed in order to make a model that would be able to use multiple different features. The largest obstacle to this was data misalignment. The available datasets lacked consistency when it came to neighborhoods and features. 

Task Two:
- A limiting factor for this task was the type of properties being evaluated. For example, a property that is an empty plot of land may have a high sale price due to square footage and location, but the absence of bathrooms and bedrooms may be misleading in determining the most influential factors.

Conclusion:
- Based on our model and evaluation, we have determined that the most important factor in residential property pricing is square footage. Despite the shortcomings of our data, we believe this would continue to be the case if more data was available.

## References:
1. Hoffman, A. (2020, December 30). *Big City Land Values and Walkscores*. Kaggle.  
   https://www.kaggle.com/datasets/alexphoffman/big-city-land-values-and-walkscores

2. Ihre, A., & Engström, I. (2019). *Predicting House prices with machine learning methods*.  
   http://www.diva-portal.org/smash/get/diva2:1354741/FULLTEXT01.pdf

3. Kulkarni, A. (2020, September 2). *Housing prices in London*. Kaggle.  
   https://www.kaggle.com/datasets/arnavkulkarni/housing-prices-in-london

4. Martin, R. (2019, December 6). *NYC Property Sales Data*. data.world.  
   https://data.world/dataquest/nyc-property-sales-data

<i>Note: This project was completed in Spring 2024 in Professor Davis's Applied Machine Learning course at Colgate University. It was completed by Anna Schwartz, Carl Ekholm, Ellie Humphreys, and Aidan Murnane. </i>

Final Poster: [https://docs.google.com/presentation/d/1SXpOjnruTxnF0uKUnE6QQIISutuMoTSqz3F8UOFsuFk/edit?usp=sharing](url)



