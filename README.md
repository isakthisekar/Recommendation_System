# Netflix Recommendation System
## Introduction
### Recommendation system
A recommendation system is a specialized type of information filtering system that analyzes large datasets to accurately identify user preferences. By understanding what users enjoy, these systems can suggest new and relevant content tailored to their interests—whether it’s movies, music, products, or even potential romantic partners.
The rapid expansion of data collection has ushered in a new era of information-driven innovation. This vast pool of data is now being harnessed to build smarter, more efficient systems—one of the most impactful being recommender systems. These systems, a subset of information filtering technologies, enhance user experience by delivering more relevant results and personalized suggestions based on user behavior and search history.
Widely adopted across industries, recommender systems power platforms such as Netflix, YouTube, Tinder, and Amazon. They analyze user preferences to present tailored content—whether it's product recommendations on Amazon, autoplay video selections on YouTube, or suggested profiles on Tinder. Social media platforms like Facebook also leverage these systems to suggest friends and pages. The effectiveness of these engines is crucial to the success of companies like Netflix and Spotify, where user engagement and satisfaction depend heavily on personalized content delivery.
### Working mechanism of recommendation system
<img width="1015" height="506" alt="image" src="https://github.com/user-attachments/assets/208bae90-2b6e-47de-80d8-ab7bbf55841c" />
### A) Understanding Relationships:

•	Relationships provide recommender systems with tremendous insight, as well as an understanding of customers. There are three main types that occur:

1) User-Product Relationship

•	The user-product relationship occurs when some users have an affinity or preference towards specific products that they need.

2) Product-Product Relationship

•	Product-product relationships occur when items are similar in nature, either by appearance or description. 

3) User-User Relationship

•	User-user relationships occur when some customers have similar taste with respect to a particular product or service.
### B) Data & Recommender Systems:-

•	In addition to relationships, recommender systems utilize the following kinds of data:

1) User Behavior Data

•	Users behavior data is useful information about the engagement of the user on the product. It can be collected from ratings, clicks and purchase history.

2) User Demographic Data

•	User demographic information is related to the user’s personal information such as age, education, income and location.

3) Product Attribute Data

•	Product attribute data is information related to the product itself such as genre in case of books, cast in case of movies, cuisine in case of food.
### C) How Do We Provide Data For Recommender Systems?

•	Recommendation engines have three basic steps to make recommendations:

1) Data Collection

•	Core of a recommendation engine is consumer data. These engines collect implicit and explicit data.

2) Data Storage

•	As the amount of data you store increases, you provide better recommendations for your customers.

3) Data Analysis and Recommendation

•	Recommendation engines analyze data by filtering it to extract relevant insights to make the final recommendations.
### Types of Recommendation Systems
<img width="1046" height="501" alt="image" src="https://github.com/user-attachments/assets/1a21bfc9-7a97-4a10-8153-8346ac79c327" />
### 1. Content-based Filtering

•	Content-based filtering methods are mainly based on the description of an item and a profile of the user’s preferred choices.

•	In content-based filtering, keywords are used to describe the items, whereas a user profile is built to state the type of item this user likes.

•	For example, if a user likes to watch movies such as Mission Impossible, then the recommender system recommends movies of the action genre or movies of Tom Cruise.

•	The critical premise of content-based filtering is that if you like an item, you will also like a similar item. This approach has its roots mainly in information retrieval and information filtering research.

### 2. Collaborative Filtering

•	The collaborative filtering method is based on collecting and analyzing information based on behaviors, activities, or user preferences and predicting what they will like based on the similarity with other users.

•	The prediction is done using various predictive maintenance machine learning techniques. For example, the k-nearest neighbor (k-NN) approach and the Pearson Correlation.

•	For example, if user X likes Tennis, Badminton, and Golf while user Y likes Tennis, Badminton, and Hockey, they have similar interests. So, there is a high probability that X would like Hockey and Y would enjoy Golf.

•	One of the main advantages of the collaborative filtering approach is that it can recommend complex items accurately, such as movies, without requiring an understanding of the item itself as it does not depend on machine analyzable content.

### Two types of collaborative filtering techniques are used:

### 1. User-User collaborative filtering:-

•	In this, the user vector includes all the items purchased by the user and rating given for each particular product.

•	The similarity is calculated between users using an n*n matrix in which n is the number of users present. The similarity is calculated using the same cosine similarity formula. The recommending matrix is calculated.

•	In this, the rating is multiplied by the similarity between the users who have bought this item and the user to which item has to be recommended.

•	This value is calculated for all items that are new for that user and are sorted in descending order. Then the top items are recommended to that user.

### 2. Item-Item collaborative filtering:-

•	In this, rather than considering similar users, similar items are considered.

•	If the user ‘A’ loves ‘Inception’ he may like ‘The Martian’ as the lead actor is similar. Here, the recommendation matrix is m*m matrix where m is the number of items present.

### 3. Hybrid Recommendation Systems

•	Hybrid Recommendation engines are essentially the combination of diverse rating and sorting algorithms. For instance, a hybrid recommendation engine could use collaborative filtering and product-based filtering in tandem to recommend a broader range of products to customers with accurate precision.

•	Netflix is an excellent example of a hybrid recommendation system as they make recommendations by:

•	Comparing the watching and searching habits of users and finding similar users on that platform, thus making use of collaborative filtering

•	Recommending such shows/movies which share common characteristics with the ones rated highly by the user. It is how they make use of content-based filtering.

•	Compared to pure collaborative and content-based methods, hybrid methods can provide more accurate recommendations. They can also overcome the common issues in recommendation systems such as cold start and the data paucity troubles.

<img width="1054" height="382" alt="image" src="https://github.com/user-attachments/assets/18d6414c-9b53-4a3f-a2a4-858eb1573232" />

## Exploratory Data Analysis (EDA)
### •	Analysis of Movies Vs TV Shows
<img width="1054" height="445" alt="image" src="https://github.com/user-attachments/assets/04880fad-e8fb-49c4-a75b-6b7576ee7a55" />
It is evident that there are more Movies on Netflix than TV shows.
### •	Month when least amount of content is added

<img width="1054" height="693" alt="image" src="https://github.com/user-attachments/assets/1f1ae3e4-2b92-4e57-8e8d-752a41741da4" />
If the year 2020 is considered, February and June were the months when comparatively less content was released. Therefore, these months may be a good choice for the success of a new release!
### •	Movie Ratings Analysis

<img width="1054" height="689" alt="image" src="https://github.com/user-attachments/assets/b8daf6a5-9270-48d6-8497-f421f4fed937" />
The largest count of movies are made with the 'TV-MA' rating. "TV-MA" is a rating assigned by the TV Parental Guidelines to a television program that was designed for mature audiences only.
Second largest is the 'TV-14' stands for content that may be inappropriate for children younger than 14 years of age.
Third largest is the 'TV-PG' rating. Programs rated TV-PG may contain some material that parents or guardians may find inappropriate for younger children. Programs assigned a TV-PG rating may include infrequent coarse language, some sexual content, some suggestive dialogue, or moderate violence.
### •	Year wise analysis

<img width="1042" height="667" alt="image" src="https://github.com/user-attachments/assets/31bd6a60-bc03-42d5-818c-1a8b83f040a1" />
Thus, 2018 was the year when most of the content were released.
### •	Analysis of TV Shows in Netflix

<img width="1046" height="580" alt="image" src="https://github.com/user-attachments/assets/8c279f73-f829-4e5c-b2d2-d32d34652f25" />
United States has the most TV Shows contents that were created in Netflix.	
### •	Analysis of duration of movies

<img width="694" height="442" alt="image" src="https://github.com/user-attachments/assets/e71b664d-e05c-4c70-82ad-2ff3616adf67" />
So, a good amount of movies on Netflix are among the duration of 75-120 mins. It is acceptable considering the fact that a fair amount of the audience cannot watch a 3 hour movie in one sitting.
### •	Analysis of duration of TV shows

<img width="726" height="576" alt="image" src="https://github.com/user-attachments/assets/427a2324-8af4-4526-81fd-0e48fac25bce" />
Thus, Grey's Anatomy, NCIS and Supernatural are amongst the tv series that have highest number of seasons.
## Content-Based Recommendation System
The TF-IDF(Term Frequency-Inverse Document Frequency (TF-IDF) ) score is the frequency of a word occurring in a document, down-weighted by the number of documents in which it occurs. This is done to reduce the importance of words that occur frequently in plot overviews and therefore, their significance in computing the final similarity score.
Term Frequency (TF), it is the relative frequency of a word in a document and is given as (term instances / total instances). Inverse Document Frequency (IDF) is the relative count of documents containing the term is given as log (number of documents/documents with term) The overall importance of each word to the documents in which they appear is equal to TF * IDF.
This will give you a matrix where each column represents a word in the description vocabulary (all the words that appear in at least one document) and each row represents a movie, as before. This is done to reduce the importance of words that occur frequently in plot descriptions and therefore, their significance in computing the final similarity score.
Fortunately, scikit-learn gives a built-in TF-IDF Vectorizer class that produces the TF-IDF matrix in a couple of lines.
With this TF-IDF matrix similarity score is computed. There are several candidates for this; such as the euclidean, the Pearson and the cosine similarity scores. There is no right answer to which score is the best. Different scores work well in different scenarios and it is often a good idea to experiment with different metrics.
We will be using the cosine similarity to calculate a numeric quantity that denotes the similarity between two movies. We use the cosine similarity score since it is independent of magnitude and is relatively easy and fast to calculate. Mathematically, it is defined as follows:

Similarity = cos(x, y) = x . y / ||x|| * ||y||
Since TF-IDF vectorizer is used, calculating the dot product will directly give the cosine similarity score.
Therefore, we will use sklearn's linear_kernel() instead of cosine_similarities() since it is faster.
Content based filtering is done on multiple factors like time, cast, director, listed in, plot, etc. the keywords are converted into lowercase and strip all the spaces between them. This is done so that our vectorizer doesn't count the Johnny of "Johnny Depp" and "Johnny Galecki" as the same. 
Soup or Bag Of Words are created for all the rows, which is strin that contains metadata that is to be fed to the vectorizer.
The  CountVectorizer() is used instead of TF-IDF because we do not want to down-weight the presence of an actor/director if he or she has acted or directed in relatively more movies. It doesn't make much intuitive sense.
Finally the recommender has been built and been capturing more information due to more metadata and has given better recommendations.

