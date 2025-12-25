# Spam Message Detection

## Dataset Overview
The spam messages dataset consists of two main columns:
- **message**: the text content of the SMS
- **label**: the class of the message, where `ham` represents a legitimate message and `spam` represents an unwanted or fraudulent message

This is a binary text classification problem aimed at identifying spam messages automatically.

## Objective
The objective is to build a machine learning model that can **classify messages as spam or ham**, helping to filter unwanted messages and improve communication security.

## Multinomial Naive Bayes (MultinomialNB)
**MultinomialNB** is commonly used for text classification tasks.  
It works by calculating the probability of a message being spam or ham based on the frequency of words appearing in each class. The model assumes word independence and selects the class with the highest probability, making it fast and effective for spam detection.

## Porter Stemmer
The **PorterStemmer** is a text preprocessing technique that reduces words to their **root or base form** (e.g., *running → run*, *messages → messag*).  
By grouping similar word forms together, it reduces vocabulary size, removes redundancy, and helps the model learn more meaningful patterns, improving classification accuracy.

## Lemmatization 
It is a text preprocessing technique that reduces words to their dictionary base form (lemma), taking context into account (e.g., better → good, running → run), which helps improve model understanding while preserving proper meaning.

---

## Results

Accuracy using stemming

![image](https://user-images.githubusercontent.com/68188457/120884545-62377280-c601-11eb-8852-a62582d6d1ee.png)


Using lemmatization

![image](https://user-images.githubusercontent.com/68188457/120884551-6f546180-c601-11eb-989d-5a57bee3d8c0.png)
