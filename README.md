# Book_recommendation_system
unsupervised Capstone Project

<b>Abstract:</b>

In this unsupervised project the main goal is to build recommender system
for users.We have provided with files such as book information like its
ISBN,publisher,title,year of book published etc.In other file which has
unique-id for users and locations,age if available.Also there is one more
file which contains explicit rating on the scale of 1-10 and explicit rating
which is expressed as 0.


<b>Problem Statement:</b>
During the last few decades, with the rise of Youtube, Amazon, Netflix,
and many other such web services, recommender systems have taken more
and more place in our lives. From e-commerce (suggest to buyers articles
that could interest them) to online advertisement (suggest to users the right
contents, matching their preferences), recommender systems are today
unavoidable in our daily online journeys. In a very general way,
recommender systems are algorithms aimed at suggesting relevant items to
users (items being movies to watch, text to read, products to buy, or
anything else depending on industries). Recommender systems are really
critical in some industries as they can generate a huge amount of income
when they are efficient or also be a way to stand out significantly from
competitors. The main objective is to create a book recommendation
system for users.

<b>Data gives us the following features:</b>

<b>Books_df:</b>

ISBN: For identifying a book's unique ISBN number.

Book-Title:Title of the book.

Book-Author:Author of the book.

Year-Of-Publication:The year in which each book was published.

Publisher:Publisher of the book.

The above features are obtained from amazon web services and in case of
several authors only first is provided.While the below given image urls are
linkings to cover pages appearing three different flavors,pointing to
Amazon website.

Image-URL-S:Image url in small.

Image-URL-M:Image url in medium

Image-URL-L:Image url in Large.

<b>Users_df:</b>

User-ID:Anonymized unique id’s for users and mapped to integers.

Location:location if provided by the user.

Age:Age of the user.

Location and age of the users are only provided if available; otherwise
these fields contain null values.

<b>Ratings_df:</b>

Ratings:Contains book rating information which is either explicitly
expressed on a scale of 1-10 or implicitly expressed by zero.

<b>Datasets:</b>

In this analysis we have used the following datasets.

➔ Books_df:This dataset contains all the information about a book like
its id,title,year of publication,publisher,etc.

➔ Users_df: This dataset contains demographic information of users by
their id’s such as location and age.

➔ Ratings_df:This dataset contains ratings of books which are either
explicit 1-10 or implicit which is 0.

<b>Steps involved:</b>

● Exploratory Data Analysis:

After loading the datasets, various analyses were performed like overview of the
data,feature Engineering.feature transformation,building recommender
engine,etc.

● Feature Engineering:

1)Handling missing values:
While exploring our project we keep in mind to handle missing values
and fill them with their respective mean or simply remove it.

2)duplicate values treatment:
Our datasets contain no duplicate values.

● Feature Transformation:

➢ Age column was fully transformed into valid ages by eliminating all
the age below 8 and above 90.
➢ In Book_df all the image urls were removed since they were of no

use for this project and for further analysis and other columns were
renamed.

➢ In User_df and Ratings_df also columns were renamed so that we
can access them easily for further operations.

● EDA Visualization:

EDA Visualization is performed by using seaborn libraries with various plots
like barplot,countplot,etc.All these plots were used to describe the
ratings,publishers,authors,etc.

TECHNIQUES:

1) K-means Clustering
2) Collaborative Filtering

1) K-Means Clustering
K-means clustering is the unsupervised machine learning algorithm that is
part of a much deeper pool of data techniques and operations in the realm
of Data Science. It is the fastest and most efficient algorithm to categorize
data points into groups even when very little information is available about
data
2) Collaborative Filtering
Collaborative Filtering is a Machine Learning technique used to identify
relationships between pieces of data. This technique is frequently used in
recommender systems to identify similarities between user data and items.
This means that if Users A and B both like Product A, and User B also
likes Product B, then Product B could be recommended to User A by the
system.

Conclusion:

● Most people know William Shakespeare but in the top 15 books by
author Agatha Christie ranks above William Shakespeare.

● JK Rowling most popular Author among teens does not make it to
the top 15 list. And also there are more books which are popular than
Harry Potter. Over the years it keeps on changing.

● Very few books have ratings 10 while most of the books are not even
rated.

● Little Women ,An American novel ranks second place in the top 15
most popular Books.

● Some Books were having more than more volumes and different
authors.

● Pride and Prejudice movie ranks in top 10 most popular books which
also have movies based on it.
