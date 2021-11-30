# udacity_project3_recommender_IBM
 
## Installation
Several libraries are used in the code file: numpy pandas matplotlib sklearn scipy pickle 

## Overview

In this work, I work to create a recommender system for users to read articles. 

Given input:

A csv file of the user-article interaction record (if a user has clicked on an article)

A csv file of the (part of) the article information database -- article id, title, description, full text.

Recommender systems based on several principles are made:

(1) **top-ranked article recommender:** Find the most popular articles to recommend

(2) **user-user based collaborative filtering:** Define user similarity, recommend articles read by similar users, rank those articles by first user-user similarity, then article popularity.

(3) **content-based recommender:** Define article similarity by first creating the document-term matrix using Tfidf Vectorizer. Article title and description are combined to create document. Then tokens are extracted and document-term matrix is created. The article-article similarity is calculated by calculating dot product of it & its transpose. For each given user, the articles that he/she has read are used to find similar articles. Then the similar articles are ranked by similarity and recommended.