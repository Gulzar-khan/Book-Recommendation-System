#CAPSTONE PROJECT OF BOOK RECOMMENDATION SYSTEM

📖Introduction:
There is a growing interest in recommender systems that suggest music, films, books, and other products and services to users based on examples of their likes and dislikes. A number of successful start-up companies like Tinder etc are also using this with big companies like Netflix, Facebook, Youtube etc,  Online book stores like Amazon and flipkart  have popular recommendation services, and many libraries have a long history of providing reader's advisory services. Such services are important since readers' preferences are often complex and not readily reduced to keywords or standard subject categories, but rather best illustrated by example.

Existing recommender systems almost exclusively utilize a form of computerized matchmaking called collaborative or social filtering. The system maintains a database of the preferences of individual users, finds other users whose known preferences correlate significantly with a given user, and recommends to a person other items enjoyed by their matched users. This approach assumes that a given user's tastes are generally the same as another user of the system and that a sufficient number of user ratings are available. Items that have not been rated by a sufficient number of users cannot be effectively recommended. Unfortunately, statistics on library use indicate that most books are utilized by very few users. Therefore, collaborative approaches naturally tend to recommend popular titles, perpetuating homogeneity in reading choices. Also, since significant information about other users is required to make recommendations, this approach raises concerns about privacy and access to proprietary customer data. Learning individualized profiles from descriptions of examples (content-based recommending), on the other hand, allows a system to uniquely characterize each user without having to match their interests to someone else's. Items are recommended based on information about the item itself rather than on the preferences of other users. This also allows for the possibility of providing explanations that list content features that caused an item to be recommended; potentially giving readers confidence in the system's recommendations and insight into their own preferences .



Objective:-

The main objective is to create a book recommendation system for users. Recommender systems are really critical in some industries as they can generate a huge amount of income when they are efficient or also be a way to stand out significantly from competitors.

📖Problem Statement

During the last few decades, with the rise of Youtube, Amazon, Netflix, and many other such web services, recommender systems have taken more and more place in our lives. From e-commerce (suggest to buyers articles that could interest them) to online advertisement (suggest to users the right contents, matching their preferences), recommender systems are today unavoidable in our daily online journeys.
In a very general way, recommender systems are algorithms aimed at suggesting relevant items to users (items being movies to watch, text to read, products to buy, or anything else depending on industries). Recommendation systems are really critical in some industries as they can generate a huge amount of income when they are efficient or also be a way to stand out significantly from competitors. The main objective is to create a book recommendation system for users.



📖Abstract:  
Recommender systems improve access to relevant products and information by making personalized suggestions based on previous examples of a user's likes and dislikes. Most existing recommender systems use social/collaborative filtering methods that base recommendations on other users' preferences. and content-based filtering  methods that uses information about an item itself to make suggestions.

📖Methods Used:-

1. Descriptive Statistics
2. Data Visualization
3. Machine Learning
4. Technologies
5. Python
6. Pandas
7. Numpy
8. Matplotlib
9. Seaborn
10. Scikit-learn
11. Surprise

📖Dataset:
The Book-Crossing dataset comprises 3 files.

1. Users : Contains the users. Note that user IDs (User-ID) have been anonymized and map to integers. Demographic data is provided (Location, Age) if available. Otherwise, these fields contain NULL values.
2. Books : Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. Moreover, some content-based information is given (Book-Title, Book-Author, Year-Of-Publication, Publisher), obtained from Amazon Web Services. Note that in the case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavors (Image-URL-S, Image-URL-M, Image-URL-L), i.e., small, medium, large. These URLs point to the Amazon website.
3. Ratings : Contains the book rating information. Ratings (Book-Rating) are either explicit, expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit, expressed by 0.

📖Project Workflow: 

1. EDA - Performed exploratory data analysis on numerical and categorical data.
2. Data Cleaning - Missing value imputation,Outlier Treaatment
3. Feature Selection - Used User-ID,ISBN and Books-Rating for model development.
4. Model development - Tried Popularity based model(for cold start), Collaborative filtering (Both Memory based and Model based) and Content-Based filtering.

Needs of this project-
1. data exploration
2. data processing/cleaning
3. recommendation system developer

📖Approach: 
We will divide this project into three systems of recommendation filtering.

As the first system we will be making some small recommendation systems to recommend books for new users(cold-start issue). we can recommend them our top selling, top rated books or our top books with weighted average ratings as well.

In the second system we will make collaborative filtering recommender. This system finds other users whose known preferences correlate significantly with a given user, and recommends to a person other items enjoyed by their matched users. This system can be divided into two types first  is model based and the second is memory based. For model based we used NMF and SVD and for memory based we build both item-item based and user-item based system.

In the third system we will build a content-based filtering. It allows a system to uniquely characterize each user without having to match their interests to someone else's. Items are recommended based on information about the item itself rather than on the preferences of other users. In this system we will make some models on the basis of books title, authors, publishers and the year of publication with the help of tags and users previous purchase history.

	
Based on these above systems we will find the best model via analyzing the results of all models by comparing with each other according to our business needs. By implementing these models efficiently we can easily recommend books to our users and it will surely helps in engaging shoppers and converting them to Customers, Increasing average order value which helps to move forward towards increasing our revenue.


📖Conclusion :

For this project our client is an online book selling firm. They now need assistance in developing a model to recommend another books on the basis of customer purchase-history and other information which are given in the datasets.

Building a model to recommend another books is extremely beneficial to the company because it can increase their sales via recommend relevant books to their customers and optimise its business model and revenue accordingly.

For modelling, it was observed that for model based collaborative filtering SVD technique worked way better than NMF with lower Mean Absolute Error (MAE) .
Amongst the memory based approach, item-item CF performed better than user-item CF because of lower computation.
Content-based recommendation on the basis of Tags are also doing good in terms of results.


Results(U-I):  Recall@5=0.23 & Recall@10=0.30

Key points:
1. Customers of age between 20 to 30 are more likely to buy books.

2. Customers who are in USA are more likely to buy books than others.

3. Our overall top selling authors are Agatha Cristie, William Shakespeare and Stephen King.

4. If we look at the ratings distribution, most of the books have high ratings with maximum books being rated 8. Ratings below 5 are few in number.

5. Our overall top selling publishers are Harlequin, Silhouette and Pocket.

6. Our overall top selling books are The Lovely Bones: A Novel, Wild Animus and The Da Vinci Code, The Red Tent (Bestselling Backlist). .

Improvements:
1. By using a marketing and advertising approach, we can reduce the age-gap.

2. We can clearly see that we have a larger number of buyer within USA, therefore we can easily recommend books to them on the basis of location and use this starategy for our campaign.

3. We nearly make 10 recommender system from which we can select Best according to our Business-needs.

4. We can push those type of books to publish which are similar to our top-selling books and recommend them to our Users.


