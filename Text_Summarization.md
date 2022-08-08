### Introduction 
Extractive text summarization does not use words aside from the ones already in the text, and selects some combination of the existing words most relevant to the meaning of the source. 
we chose various articles with different categories  after that we  make  preprocessing  .
we applied Summrization Model like Bert and LSA .

**Table of Contents**

[TOCM]

[TOC]
#Implement Steps 
#Preprocessing
our divides into label, text, and text summary after we look at this data we find this data is useful for our needs.
 but like any data, there are many characters not useful  so we started to clean the data 
 from any unwanted characters, white spaces, and stop words. we lemmatized  and stemmed but we keep commas and full stops 
#Split data
  Splitting the data into cleaned text that include only text  after cleaning it  with their labels
#Perform Feature Engineer
 it is very important tb be able to deal with model by help us convert text sentences into numeric vectors.
####BOW
The Bag of Words is a method often used for document classification. This method turns text into fixed-length vectors by simply counting the number of times a word appears in a document, a process referred to as vectorization.
As we said that we split the data. So, we applied BOW to training and testing data.
####Tf-IDF
Term frequency works by looking at the frequency of a particular term you are concerned with relative to the document. There are multiple measures, or ways, of defining frequency
As we said that we split the data. So, we applied Tf-IDF to training and testing data.
#Classfication
####SVM
Support vector machines are a set of supervised learning methods used for classification, regression, and outliers detection. All of these are common tasks in machine learning.
 we applied  it  with Bow  and give the accuracy 93%
  and with Tf-idf 95%
#### Decision Tree
Decision Tree is the most powerful and popular tool for classification and prediction. A Decision tree is a flowchart-like tree structure, where each internal node denotes a test on an attribute, each branch represents an outcome of the test, and each leaf node (terminal node) holds a class label. 
 we applied it  with Bow  and give the accuracy 86%
  and with Tf-idf--
#### KNN
The k-nearest neighbors (KNN) algorithm is a simple, easy-to-implement supervised machine learning algorithm that can be used to solve both classification and regression problems. 
 we apply it  with Bow  and give the accuracy 69%
  and with Tf-idf--
#### MLP
#Clustering
####K-means
Centrid-based Clustering .K-means is an unsupervised machine learning algorithm in which each observation belongs to the cluster with the nearest mean.
 We applied it with BOW and Tf-idf
####Agglomerative
Connectivity_based clustering .the most common type of hierarchical clustering used to group objects in clusters based on their similarity.
 We applied  it with BOW and Tf-idf
#Summrization Technique 
####Bert
BERT is the encoder of transformers, and it consists of 12 layers in the base model, and 24 layers for the large model. So, we can take the output of these layers as an embedding vector from the pretrained model.
There are three approaches to the embedding vectors: concatenate the last four layers, the sum of the last four layers, or embed the full sentence by taking the mean of the embedding vectors of the tokenized word
####LSA
#Chatbot
Question and answering system  that extracts the answer from the text summary from Bert and LSA 
#Innovation 
We created a transformer model to translate   the text  to Arabic, German, and  Chinese
#Conclusion
In this project, we applied data pre-processing, classification techniques, and clustering. Then we applied LSA and Bert summarization models, after that we made a comparison between them.
The LSA model had a good sores and summary close to the human summary than the BERT model.
After that we made the error analysis to see what the machine tried to predict.
Then we made a simple question and answering system, to extract the answer from the summary.
Finally, we made a different language translation from English to German, Chinese, and Arabic languages.
