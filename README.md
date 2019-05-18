# Sentiment-Analysis-on-Online-Product-Reviews
The objective of this project is to classify whether upcoming product will have positive or negative Sentiment.   


![alt text](https://github.com/shreyaswankhede/Sentiment-Analysis-on-Online-Product-Reviews/blob/master/s1.png
 "Correlation between features")

***

# Sentiment Analysis:

* Sentiment analysis and Opinion mining is the computational study of User opinion to analyze the social, psychological, philosophical, behavior and perception of an individual person or a group of people about a product, policy, services and specific situations using Machine learning technique. Sentiment analysis is an important research area that identifies the people’s sentiment underlying a text and helps in decision making about the product.

# Customer Product reviews:

* A customer review is a review of a product or service made by a customer who has purchased and used, or had experience with the product or service. Customer reviews are a form of customer feedbacks on electronic commerce and online shopping sites. 
90% of consumers read online reviews before purchasing product and 88% of consumers trust online reviews as much as personal recommendations.

****

# Objective:

<h3>End-user:</h3> E-Commerce Organization
<h3> Dataset:</h3> 
The Online Product Reviews dataset includes following features:
Dependent feature: reviews.rating (Unhappy,OK,Happy)
Independent features: review.text (Reviews)
The dataset contains 71044 rows and 25 columns

* Source: https://data.world/datafiniti/grammar-and-online-product-reviews

***

# Workflow:

![alt text](https://github.com/shreyaswankhede/Sentiment-Analysis-on-Online-Product-Reviews/blob/master/s2.png
 "Correlation between features")

<h2> Steps: </h2>
<br>1. Data loading.
<br>2. Data Preprocessing

* Remove Punctuations,special symbols and special characters.

* Stopword Removal

* Tokenization

* Stemming

***

# WordCloud:

![alt text](https://github.com/shreyaswankhede/Sentiment-Analysis-on-Online-Product-Reviews/blob/master/s4.png
 "Correlation between features")

# Feature Extraction:

* In order to make sense to our machine learning algorithm we have converted each review to a numeric representation which is called 'Vectorization'.

* The system uses TF-IDF Vectorizer (Term Frequency-Inverse document frequency) that transforms a count matrix to a normalized frequency representation in float.

* Splitting the data into Train and Test set (70-30).


<br> 1. TF-IDF

1.Count how many times does a word occur in each message (Known as term frequency)
2.Weigh the counts, so that frequent tokens get lower weight (inverse document frequency)

<br>TF(t) = (Number of times term t appears in a document) / (Total number of terms in the document).
<br>IDF(t) = log_e(Total number of documents / Number of documents with term t in it).

* Example: Consider a document containing 100 words wherein the word dog appears 3 times. The term frequency for dog is (3 / 100) = 0.03. Assume total of 10 million documents and the word dog appears in one thousand of these. Then, the inverse document frequency is calculated as log(10,000,000 / 1,000) = 4. 

* Thus, the Tf-idf weight is the product of these quantities: 0.03 * 4 = 0.12.

***

# Model Building:
<br> Building Support Vector Machine (SVM) and SGDClassifier on feature vectors.

# Results:
![alt text](https://github.com/shreyaswankhede/Sentiment-Analysis-on-Online-Product-Reviews/blob/master/s5.PNG
 "Correlation between features")

***


<br>Thank You!	
<p><!-- Place this tag where you want the button to render. -->
<a class="github-button" href="https://github.com/shreyaswankhede" aria-label="Follow @shreyaswankhede on GitHub">Follow @shreyaswankhede</a>

