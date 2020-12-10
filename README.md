### Overview

Welcome to `Ji Yoon's & Mariana´s sentiment analysis project`, 
here you will be able to find everything related to our Initial Project Report 
(so far) inlcuiding datasets and the first attempts we will be implementing
in order to perform a tweet sentiment analysis on tweets related to `Covid19`.

### Dataset
The Data set is from Aman Miglani (Coronavirus tweets NLP - Text Classification: Corona Virus Tagged Data) 

### Steps
The steps we are planning to take are the following ones:

#### Initial Project report
1. Search and load necessary libraries
2. Tweet pre-processing
3. Exploratory data analysis
  + Here we want to explore the distribution of the tags in the training and the test data sets
  + If possible, to plot the evolution of sentiments through time
  + Create a visual representation of most common words and hashtags

For this report, the main challenges we faced were regarding the tweet processing. 
First, we tried with a function that cleaned the tweets but was only able to be applied to a vector and not as part of the data frame. 
Then, we defined another function that actually cleans the database but does not run on jupyter notebooks, only locally. 
That is why the histogram of the HT cannot be displayed. We still need to figure out how to homologate that in order to make everything 
run properly and with the same function of cleaned tweets. For example, the wordclouds work with the function we specify inside the same code section, 
but this does not apply to the whole data frame, only for the wordcloud. 

#### Final Project report
4. Tokenization
5. Model Construction
6. Analysis of key findings & final presentation

For the final project report, the main challenges we faced were regarding the vectorization and the model construction. We vectorized the tokenized data using two different methods: Bag of Words (BoW) and TF-IDF. The BoW vectorizer creates a matrix of tokenized words and is the simplest way to represent text by numbers. A key drawback of BoW is that it retains no information about the order or significance of words. This can be problematic when dealing with negations. The TF-IDF method, the most popular method, basically calculates how important a word is to a document. Words with higher scores are more important and vice versa.

When trying both methods in our code, we ran into some challenges. While the Bag of Words vectorization method worked, the TF-IDF method returned some error codes we have been unable to work through. This is unfortunate because TF-IDF method provides more information and is more widely used in NLP. 

Using the vectorized data given by the BoW method, we plugged it into two different models. First we tried a ridge regression classifier, which has a slight advantage over our second model, logistic regression, because it is able to give bias to more important variables, whereas logistic regression treats all variables equally. The ridge regression model yielded an accuracy rate of approximately 54%. The logistic regression classifier had an accuracy rate of approximately 50%, slightly less accurate than ridge regression. Neither of these were ideal. 

We sought to improve the accuracy by trying the Random Forest classifier which initially worked but stopped working suddenly. However when it worked it yielded an accuracy rate of 96%, which is much more preferable. However, as Huy suggested, it was mainly because we were not splitting correctly the train/test data. We decided not to include this in the final report.
