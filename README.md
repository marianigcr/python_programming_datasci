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
  + Defining embedding dimension
  + Building sequential neural network
  + Compiling and training model
  + Evaluate model
  + Calculate and plot confusion matrix
  + Print Clasification report
6. Analysis of key findings & final presentation

