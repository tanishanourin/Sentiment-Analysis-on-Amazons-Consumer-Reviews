# COMP6200 Data Science

# Project Proposal

## Sentiment Analysis of Amazon&#39;s Consumer Reviews

Sentiment analysis is the process of detecting positive or negative sentiment in text. It&#39;s often used by businesses to detect sentiment in social data, gauge brand reputation, and understand customers. Since customers express their thoughts and feelings more openly than ever before, sentiment analysis is becoming an essential tool to monitor and understand that sentiment. Automatically analyzing customer feedback, such as opinions in survey responses and social media conversations, allows brands to learn what makes customers happy or frustrated, so that they can tailor products and services to meet their customers&#39; needs.

## Data Source and Background:

Data, we will use is a list of over 28k consumer reviews for Amazon products like the Kindle, Fire TV Stick, and more provided by Datafiniti&#39;s Product Database. The dataset includes basic product information, rating, review text, and more for each product.

The dataset which we are going to use is from [Dataworld.com](https://data.world/datafiniti/consumer-reviews-of-amazon-products#)

## Project Goal:

- Perform data preprocessing to prepare the text data for analysis and modeling.
- Build Machine Learning models to classify text as either positive, negative or neutral sentiment.
- Visualize how the products are rated according to their score (rated by the customers for each product) and what are the most reviewed Amazon products?
- Which amazon product has highest positive reviews?
- How many negative responses for a particular amazon product?
- Which amazon product has highest positive reviews after a certain period of time of its launch date?
- Variation of the reviews after a product launch compare to the days available for sale.

## Data Format:

The dataset provided by data.world is in CSV format.

## Techniques expected to use in the project:

- We expect to use scikit-learn software, an open-source machine learning software package in Python for model fitting, data pre-processing, model selection and evaluation, and many other utilities.
- Naïve Bayesian and Random Forest for classification models selected for categorization
- NLTK Python package for building common algorithms such as tokenizing, part-of-speech tagging, stemming, sentiment analysis, topic segmentation, and named entity recognition.
- Logistic Regression to find weighted combination of variables that best predicts a response.
- Support Vector Machine (SVM) linear model with a stochastic gradient descent (SGD) optimizer for text classification and natural language processing.

## Project Plan:

**1.Data Cleaning and Visualization:**

For initial data processing we need to clean the dataset by removing columns which are not relevant to our analysis, deal with NaN values by removing or performing imputations and any row having data in any other type than string we will change that to a string for review column. Visualize column variables using bar plots, box plots or histograms for categorical variable.

**2.Data preprocessing:**

After data cleaning, our next approach is dealing with our unstructured text data through Natural Language Processing to make it more usable, as machine learning algorithms do not work with raw text directly. The process includes:

1. Lowercasing Texts
2. Tokenizing sentences to break text down into sentences, words, or other units.
3. Stemming and Lemmatization
4. Stop word removal: Removing stop words like &quot;if,&quot; &quot;but,&quot; &quot;or,&quot; and so on.
5. Normalization: Normalizing words by condensing all forms of a word into a single form.
6. Noise removal (Punctuation marks, special characters etc. using Regular Expressions)
7. Vectorizing text by turning the text into a numerical representation for consumption by your classifier using Bag-of-Words/TF-IDF technique

**3.Building classification model:**

We will start withsplitting data into training and evaluation sets, train the classifiers using the train dataset and evaluate the model performance with test dataset. For improving performance, we will use complex models like naïve bayes classifier and support vector machine.

**4. Evaluation:**

We will evaluate our model using metrices such as classification accuracy, Confusion matrix, F1 score, ROC curve and AUC.

## Preliminary Exploration of The Data

![Images](/Images/Graph.PNG)

Average words/review - ~26

Skewness - ~14.2

Preliminary exploration of the datasets shows uneven distribution of frequency of words in text reviews which may affect the efficiency of the model

## Project Milestones:

Week 10 # Preprocess the dataset using Natural Language processing for analysis.

Week 11 # Build a classifier and perform sentiment analysis.

Week 12 # Improve performance and evaluate the model.
