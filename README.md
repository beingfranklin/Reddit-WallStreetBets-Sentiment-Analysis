# Sentiment analysis of r/wallstreetbets during the GameStop saga

This project, done as part of university coursework, uses Sentiment Analysis to examine the correlation between GameStop($GME)’s stock price and the massive surge in social media attention that the organisation experienced.

## Objectives

* Examine timeline of events to identify a particularly relevant timeframe.
* Conduct in-depth exploration of the obtained dataset to gain context.
* Use multiple machine learning models to predict polarity to individual posts.
* Compare frequency of different polarity with movement of stock price, generating an aggregated visual representation of this interaction and use this information to evaluate our hypothesis. Are they correlated?
* Evaluate the output and accuracy of each machine learning model.
* Assess limitations of our analysis and suggest improvements that can be made for future iterations of these methods.

## Datasets

* **reddit_wsb.csv** - For prediction, we are using reddit_wsb.csv, a substantial set containing nearly 45,000 posts drawn from the week after Musk’s tweet from Kaggle. Attributes are:

| title | score | id  | url | comms_num | created | body | timestamp |
|-------|-------|-----|-----|-----------|---------|------|-----------|

* **Reddit_wsb_labelled.csv** - For training and testing our models, we will be using Reddit_wsb_labelled.csv, which provides large set of posts with associated polarity. Attributes are:

| clean_comment | category |
|---------------|----------|

* **Tingo API** - To gather GME’s historical stock price data we used the financial research API *Tiingo* to download the ticker values of the stock from the 28th January 2021 to the 5th February 2021.


## Notebooks

There are mainly two Jupyter notebooks included in this repository

* **Data_Exploration.ipynb** -  This notebook contains the data exploration that was done as part of this project.
* **ML_Models.ipynb** -  This notebook contains the ML Models and other analysis that was done as part of this project. Logistic Regression, Linear SVC and Multinomial Naïve Bayes were the models used. This file also contains comparison of these models, their confusion matrix and other relevant visualisations.

*P.S. -  Read the **Report.pdf** to know more about this project and conclusions*.


## Authors

* **Franklin Antony** (MSc Computer Science, QMUL)
* **Alexander Murphy** (MSc Computing & Information Systems, QMUL)

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss.

## License
[MIT](https://choosealicense.com/licenses/mit/)
