# recommendation-system
Welome to Recommendation Systems! I've designed this repo to expand your knowledge of recommendation systems and explain collaborative filtering model used in recommendation

# What are Recommendations?

- How does YouTube know what video you might want to watch next?
- How does the Google Play Store pick an app just for you?

Magic? No, in both cases, an ML-based recommendation model determines how similar videos and apps are to other things you like and then serves up a recommendationns

# Why Recommendations?

A recommendation system helps users finding compelling content in a large corpora. For example, the Google Play Store provides millions of apps, while YouTube provides billions of videos. More apps and videos are added every day. How can users find new compelling new content? 

Yes, one can use search to access content. However, a recommendation engine can display items that users might not have thought to search for on their own.

# Terminology
Before we dive in, there are a few terms that you should know:

### Items
- The entities a system recommends.
- For the Google Play store, the items are apps to install.
- For YouTube, the items are videos.
- For Spotify, the items are music.
- also known as documents

### Query
The information a system uses to make recommendations, also known as context

Queries can be a combination of the following:
- user information
- the id of the user
- items that users previously interacted with
- additional context
- time of day
- the user's device

### Candidate generation
It is the first stage of recommendation. 
- Given a query
- The system generates a set of relevant candidates.

The following table shows two common candidate generation approaches:

| Type        | Definition           | Example  |
|:-------------------:|:-------------------:|:-----------:|
| content-based filtering	      | Uses similarity between items to recommend items similar to what the user likes. | If user A watches two cute cat videos, then the system can recommend cute animal videos to that user. |
| collaborative filtering	      | Uses similarities between queries and items simultaneously to provide recommendations.| If user A is similar to user B, and user B likes video 1, then the system can recommend video 1 to user A (even if user A hasn’t seen any videos similar to video 1).
 

# Collaborative Filtering
To address some of the limitations of content-based filtering, collaborative filtering uses similarities between users and items simultaneously to provide recommendations.

This allows for serendipitous recommendations; that is, collaborative filtering models can recommend an item to user A based on the interests of a similar user B. Furthermore, the embeddings can be learned automatically, without relying on hand-engineering of features.

This notebook covers the following collaborative filtering based approaches:

- User-based CF (cosine)
- User-based CF (pearson correlation)
- Item-based CF (cosine)
- Item-based CF (adjusted cosine)

# Types of Collaborative Filtering models

## Nearest neighbor Collaborative Filtering:

- These type of recommendation systems recommend based on nearest neighbors
- Nearest neighbor approach is used to find out either similar users or similar products,

It can be looked at two ways,

### User based filtering
- Find the users who have similar taste of products as the current user
- Similarity is based on purchasing behavior of the user
- So based on the neighbor purchasing behavior we can recommend items to the current user.

### Item based filtering
- Recommend Items that are similar to the item user bought
- Similarity is based on co-occurrences of purchases
- Item A and B were purchased by both users X and Y then both are similar.

![Nearest neighbor collaborative filtering](https://miro.medium.com/max/875/1*8Ex4Vyb7dFOIlqGS2Q1Eiw.jpeg "Nearest neighbor collaborative filtering")
Image source from [here](https://medium.com/@cfpinela/recommender-systems-user-based-and-item-based-collaborative-filtering-5d5f375a127f)
# Matrix factorization:
- It is basically model based collaborative filtering
- Matrix factorization is the important technique in recommendation system.

An abstractive explanation for matrix factorization,
- When a user gives feed back to a certain movie they saw (say they can rate from one to five)
- this collection of feedback can be represented in a form of a matrix
- Each row represents each users, while each column represents different movies
- Obviously the matrix will be sparse since not everyone is going to watch every movies, (we all have different taste when it comes to movies).

![Matrix Factorization](https://miro.medium.com/max/875/1*kxAP7W7aOGdcgpTFUMgSfg.jpeg "Matrix Factorization")
Image source from [here](https://www.youtube.com/watch?v=ZspR5PZemcs)


# TODO

- Matrix Factorization
- Deep Neural Networks.
