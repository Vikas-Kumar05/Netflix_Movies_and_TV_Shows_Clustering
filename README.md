# Netflix_Movies_and_TV_Shows_Clustering
![image](https://github.com/vks2268/Netflix_Movies_and_TV_Shows_Clustering/assets/117895012/e9aeb912-4707-4cec-9665-9c1ccee94118)

# Introduction

Introduction Netflix, the world’s largest on-demand internet streaming media and online DVD movie rental service provider.it Founded August 29, 1997, in Los Gatos, California by Marc and Reed. It has 69 million members in over 60 countries enjoying more than 100 million hours of TV shows and movies per day Netflix is the world’s leading internet entertainment service with enjoying TV series, documentaries, and feature films across a wide variety of genres and languages. I was curious to analyze the content released in Netflix platform which led me to create these simple, interactive, and exciting visualizations and find similar groups of people.

# Problem Statement

This dataset consists of TV shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.
Integrating this information with additional external datasets such as IMDB ratings and rotten tomatoes can yield a plethora of fascinating results.

# Data Summary

The dataset had 12 attributes and around 7787 records. To get started, we mounted the drive, imported the required libraries, and stored the data in variables. We separated the date added column into days, months, and years as the next stage in the data wrangling process.

The next phase was data analysis and visualisation, where we looked at our data distribution using various plots and attempted to draw useful conclusions from the dataset.

We performed feature engineering and data pre-processing to prepare the data for model training. We dealt with the null values by appropriately replacing them.

We choose to cluster the data based on the attributes director, cast, country, genre, rating, and description during the preprocessing of the textual data. The stopwords and punctuation were all eliminated after choosing the attributes for clustering. We used SnowballStemmer to conduct stemming on these properties after changing their case to lowercase.

These attributes' values underwent tokenization, preprocessing, and vectorization using TFIDF vectorizer. The total number of characteristics we produced through TFIDF vectorization was 10000.

To lessen the dimensionality, we employed Principal Component Analysis (PCA). With the use of the scree plot, we saw that approximately 5000 components could account for more than 90% of the variation; as a result, the number of components was limited to 5000.

The K-Means Clustering technique was used to build the initial clusters, and 10 clusters were determined to be the ideal number. Elbow technique and Silhouette score analysis were used to obtain this.

The Agglomerative clustering technique was then used to create clusters, and it was discovered that 14 clusters were the most effective number. The dendrogram was visualised to obtain this.

The similarity matrix acquired after utilising cosine similarity was used to construct a content-based recommender system. Based on the sort of show the user viewed, this recommender system will provide them with 10 recommendations.

Overall, we used a combination of Data Processing, Visualization, and Machine Learning Methods while working on this specific dataset. Although it was a difficult undertaking, we were able to develop clusters and a content-based recommender system using the proper strategy.

# Conclusion

it will solve for improved movie and TV-Show selection times with a considerable growth in satisfaction of the content being consumed leading to more user engagement and greater trust in Netflix recommendations.
