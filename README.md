# Book-Recommendation-System
Unsupervised ML Capstone Project : Book Recommendation System
# About Project
The project concerns the books recommendation system. It includes data analysis, data preparation and explored three kind of recommendations - the simplest recommendations, content-based filtering and collaborative filtering (KNN model and matrix factorization). The final result will show that the user can input one book's name or author then the system can provide the other most possible books that he can to read.
# Motivation
The Recommendation System is based on previous (past) behaviours, it predicts the likelihood that a user would prefer an item. Many of applications for example Netflix uses recommendation system. It suggests people new movies according to their past activities that are like watching and voting movies. The purpose of a book recommendation system is to predict buyer’s interest and recommend books to them respectively. That system can take into regard many parameters like book content and quality by filtering user reviews.
# Dataset Information
Dataset used in this project is the Amazon Book-crossing dataset.This dataset has been compiled by Cai-Nicolas Ziegler in 2004, and it comprises of three file.They are:

**Users**
* User-ID: A unique identification number for each user
* Location:It contains city,state and country to which the user belongs ,separated by commas
* Age:The age of the user
  
**Books**
* ISBN:International Standard Book Number unique to each edition of the book
* Book-Title:Title of the book
* Book-Author:Author of the book(incase of several authors only the first is provided)
* Year-of-Publication:The year in which the particular edition of the book was published
* Publisher:Name of the Book Publishing company
* Image-URL-S: URL link to a small version of the book cover displayed on the Amazon website
* Image-URL-M: URL link to Medium version image of the book cover displayed on the Amazon website
* Image-URL-L: URL link to Large sized image of the book cover displayed on the Amazon website
  
**Ratings**
* User-ID:as mentioned above
* ISBN:as mentioned above
* Book-Rating: The rating given by the user (identified by User-ID) for the book (identified by ISBN). It is either explicit,expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit,expressed by 0.

# Steps Involved
* **Data Preprocessing :** Checked for outliers, incorrect values, missing values, duplicate, performed data type correction and string formatting.
* **Merging of datasets :** In this project, recommender systems were built utilizing only explicit ratings . So finally,a new dataframe by merging the books dataset ,explicit ratings dataset and users dataset.
* **Feature Extraction :** Created new columns such as age_group by binning the 'Age' column and extracted the country name from the 'Location' column .
* **Exploratory Data Analysis :** Performed Univariate, Bivariate, and Multivariate analysis with various graphs and plots to better understand the distribution of features and their relationships.
* **Implementation of various Recommender System approaches**

# Approaches used
The approaches used in this project are:

1. Popularity Based recommendation system
It is a type of recommendation system that bases choices on factors like popularity and/or current trends. These systems determine which item (in this case,books) are in the trending list or are the most well-liked by users and then directly recommend them.

* Weighted average rating approach
* Country-wise approach
* Author-wise approach
2. Collaborative Filitering Based recommendation system
The Collaborative Filtering approach first investigates the user’s behaviors, interests, and searches for similar users. It recommends items to users based on the ratings of similar users on various items and by predicting the missing ratings of the items . CF is broadly classified as memory-based and model-based CF.

* Memory Based approach - KNN (similarity between items)
* Model Based approach- SVD based recommendation system (prediction of ratings)

# Conclusion
* The Lovely Bones: A Novel and Wild Animus are the two most read books.
* Stephen King is the most popular book author based on the number of ratings.
* Ballantine Books and Pocket are the top publishers based on the number of ratings that their books have received.
* The majority of readers are between the ages of 25 and 40.
* The majority of readers who have given the books ratings are from the United States and Canada.
* Regardless of the age group, The Lovely Bones and Wild Animus appear on lists of the top-rated books.
* We have built five types of recommendation systems and did evaluation for one of them.
* In the case of Memory-based approach, the Cosine similarity-based KNN performs better at recommending books that are similar than the Euclidean distance-based KNN.
* After evaluation for Collaborative-Model Based Recommendation system, we got a recall@5 of 30% and recall@10 of 41%.

