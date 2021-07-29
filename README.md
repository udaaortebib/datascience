# datascience
Udacity Data Scientist 1st Project

Link to project blog post:
https://hakon-doksrod.medium.com/analysis-and-prediction-of-airbnb-prices-in-seattle-12115d639887

Installation:
This project requires Python 3.x and the following Python libraries installed:

    NumPy
    Pandas
    matplotlib
    scikit-learn
    Jupyter-Notbook

Data files: (Data publicly available here: https://www.kaggle.com/airbnb/seattle)

    listings.zip
    reviews.zip Notebooks:
    airbnb_neighborhood.ipynb
        Exploration and analysis of prices and variation of prices between different neighborhoods of Seattle
    airbnb_prediction.ipynb
        Building a model for price prediction using machine learning techniques.

Motivation:
This project is a part of my Udacity Data Scientist Nanodegree program. I chose to work with Airbnb data from Seattle. I was interested in exploring and analyzing prices of AirBnB listings and how they vary depending on neighborhood. Furthermore, I was interested to explore how difference in price was reflected in how properties are described/reviewed.

I also wanted to try to build a model for predicting the price of listings using machine learning. Being my first attempt at building this kind of model, I expected this to be challenging, but ultimately a good learning experience.

Summary of results:
The first part of the analysis, regarding prices and variation between neighborhoods, yielded findings that largely pointed towards location being important to the price level of the listing. Looking further into reviews and descriptions of listings in the most and least expensive neighborhoods also revealed that location seems to be given more importance in the description of listings in the most expensive neighborhoods, and more on the property itself in the least expensive neighborhoods.

I first built a linear regression model for predicting price, which gave quite mediocre results with an R squared score of aboubt 0.63. Using a gradient boosting regressor I was able to increase the score to about 0.70, which is still not great but at least a decent score. Looking more closely at results and residuals, the models were clearly not very good at predicting prices in cases of expensive listings. This was not unexpected, as the models didn't have a lot of these kinds of listings in the dataset to train with.

Acknowledgements:
Several of the functions used in building the prediction models were taken or adapted from functions used in the Udacity course.
Webites used for code solutions/inspiration:
https://www.w3resource.com/python-exercises/list/python-data-type-list-exercise-183.php https://towardsdatascience.com/how-to-generate-prediction-intervals-with-scikit-learn-and-python-ab3899f992ed https://nbviewer.jupyter.org/github/WillKoehrsen/Data-Analysis/blob/master/prediction-intervals/prediction_intervals.ipynb https://www.datacamp.com/community/tutorials/wordcloud-python
