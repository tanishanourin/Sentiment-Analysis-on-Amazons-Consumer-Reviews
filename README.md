# Macquarie University 
# COMP 6200 - Data Science 
# project-group-12

## Topic : Sentiment Analysis of Amazon's Consumer Reviews

<p align="center">
<img width="560" height="400" src=/Images/Introduction-Image.jpg
</p>
  
  
 **Group Members:**

**(1)Abhishek Singh** 46339868

**(2)Arzoo Nayeem** 46218858

**(3)Harsimranjeet Singh** 46238301

**(4)Tanisha Nourin Alam** 46159770
  
  
**Dataset:**  

  For the dataset used in the project refer to this link == > [Amazon Consumer Reviews](https://query.data.world/s/kxpnmeeabp2sv7wiuo7td57bfgecap)

**1. Data Exploration :**

* Exploring Shape of data 
* Checking missing/null values
* Finding Summary Statistics of Numerical features using describe function
* Exploring Count of words/review for each product using graph
  
<p align="center">
<img width="560" height="400" src=Images/Count_of_words.png
</p>   

 <p align="center">
    Fig.1 Highest reviewd Amazon Products
</p> 
  
* Exploring Percentage distribution of rating in data 


* Generating wordcloud for reviews
<p align="center">
<img width="560" height="400" src=/Images/reviews_wordcloud.png
</p>  
  <p align="center">
    Fig.2 High Frequency Words in Customers Review
</p>

**2) Visualization :**

Different graphs are plotted to get information about different products and their reviews like which are most reviewed products, count of words in review, deep diving in some particular products to see behaviour of customers towards that product.

 2.1 Reviewer's rating distribution among products:
 
 2.2 Exploring number of reviews for top 20 products
  
 <p align="center">
<img width="560" height="800" src=/Images/Reviews_for_Top_20_Products.png
</p>
  
 <p align="center">
    Fig.3 Top 20 products with highest reviews
</p> 


   

 
 2.3 The most reviwed amazon products
 
 2.4 The highest positive reviews:
 
 2.5 Negative Reviews for products
 
 2.6 Performance of amazon products in particular timeline (Comparing with the launch date as of dataset)
 
**3. Pre processing of Data :**

Applied data cleaning techniques : 

* Lower casing - Lowercasing ALL your text information, albeit normally neglected, is one of the easiest and best type of text preprocessing. It is pertinent to most content mining and NLP issues and can help in situations where your dataset isn't huge and altogether assists with consistency of expected output.

* Removal of Stopwords - Stop words are a bunch of regularly utilized words in a language. Instances of stop words in English are "a", "the", "is", "are" and so forth The instinct behind utilizing stop words is that, by eliminating uninformed words from text, we can zero in on the significant words all things being equal.

* Removal of special characters - Special characters and images are normally non-alphanumeric characters or even sporadically numeric characters (contingent upon the issue), which add to the additional noise in unstructured content.

* Removal of Emoticons - Not all emoticons pass on the message. A significant number of them are insignificant. we should eliminate it as they are not giving any accommodating data.
To remove all emoticons, Download a list of emoticons which covers all expressions and can apply the same function into text data.

* Normalization : Normalise text is really lessening events of a token so it gets addressed by a solitary rendition of this token.The   equivalent happens to plural words, which can be addressed by their singular variant. Truth be told, we don't actually mind what finishing that word has. 

There are two different ways to standardize tokens. They are called stemming and lemmatization.

 a) Stemming - Stemming is the process of reducing inflection in words to their root form. It uses a crude heuristic process that chops off the ends of words in the hope of correctly transforming words into its root form.It works by cutting off the end or the beginning of the word, taking into account a list of common prefixes and suffixes that can be found.
 
 b) Lemmatization - Lemmatization is important and more ‘correct’ from a grammatical standpoint, since it takes irregular words and plural into account.

**4) Building the Models :**

 4.1 Train test split
 
 4.2 Feature extraction using TfidfVectorizer
 
 4.3 Model Building
 
  4.3.1 Model 1: Logistic Regression
  4.3.2 Model 2: Multi-layer Perceptron classifier
  
 4.4 Comparison of Models
   
 <p align="center">
<img width="560" height="400" src=/Images/Comparison_of_Models.png
</p>
  
 <p align="center">
    Fig.4 Comparison Between Models
</p> 
 
 
 
 4.5 Business Perspective
      
 <p align="center">
<img width="560" height="400" src=/Images/ROC_Curve.png
</p>
  
 <p align="center">
    Fig.5 ROC Curve
</p> 
 
  
   
  From the above curve, it implies which is the better model according to out dataset and therefore MLP is better model than Logistic    Regression.
  
**5) Appendix :**

  5.1 Model 1: Naive Bayes (Multinomial)
  
  5.2 Model 2: Decision Tree Classifier
  
  5.3 Word2Vec
  
  5.4 Comparison
      
<p align="center">
<img width="560" height="400" src=/Images/Models.png
</p>
<p align="center">
    Fig.6 Comparison Between Models
</p>
 
**Conclusion:** To Overcome the issue of overfitting and biased classification different models were implemented and we conclude that Multilayer perceptron is performing comparatively better while classifying the negative classes(Imbalance Class)  

