![Netflix](https://github.com/aakashr21/Netflix-movies-and-tv-show-clustering/assets/88080322/2c716c01-31c8-41c8-aeb0-3560433fc752)

# Netflix Movies and TV Shows clustering

The goal of this project is to analyze the Netflix catalog of movies and TV shows, which was sourced from the third-party search engine Flixable, and group them into relevant clusters. This will aid in enhancing the user experience and prevent subscriber churn for the world's largest online streaming service provider, Netflix, which currently boasts over 220 million subscribers as of 2022-Q2. The dataset, which includes movies and TV shows as of 2019, will be analyzed to uncover new insights and trends in the rapidly growing world of streaming entertainment.


## Insights
* There are totally 7787 contents in netflix in this 30.95% is TV Shows and 69.05% is movies.
* The most number of movies are directed by Raúl Campos, Jan Suter.
* The most number of TV shows are directed by Alastair Fothergill.
* United States has released most number of movies and TV shows.
    * 1850 movies and 705 TV shows are released in United States.
* India is second country which has released most number of movies, totally 852 movies.
* After year 2017 more contents have added in netflix compared to other years.
* In netflix more contents are added between september and janurary.
* Population and production of TV show is increased after year 2015.
* In netflix adult and teen ratings contents are more
    * Movie: TV-MA:1845 , TV-14:1272
    * TV shows: TV-MA:1018 , TV-14:659
* The common duration for movies is 90 mins and for TV shows is 1 season.
## Conclusion
In this project, we tackled a text clustering problem in which we had to categorize and group Netflix shows into specific clusters in such a way that shows in the same cluster are similar to one another and shows in different clusters are not.

There were approximately 7787 records and 11 attributes in the dataset. We started by working on the missing values in the dataset and conducting exploratory data analysis (EDA). It was discovered that Netflix hosts more movies than television shows on its platform, and the total number of shows added to Netflix is expanding at an exponential rate. Additionally, most of the shows were made in the United States. The attributes were chosen as the basis for the clustering of the data: cast,genre, director, rating, and description The TFIDF vectorizer was used to tokenize, preprocess, and vectorize the values in these attributes. 10000 attributes in total were created by TFIDF vectorization. The problem of dimensionality was dealt with through the use of Principal Component Analysis (PCA). Because 4000 components were able to account for more than 80% of the variance, the total number of components was limited to 4000. Utilizing the K-Means Clustering algorithm, we first constructed clusters, and the optimal number of clusters was determined to be 5. The elbow method and Silhouette score analysis were used to get this. The Agglomerative clustering algorithm was then used to create clusters, and the optimal number of clusters was determined to be 5. This was obtained after visualizing the dendrogram. The similarity matrix generated by applying cosine similarity was used to construct a content-based recommender system. The user will receive ten recommendations from this recommender system based on the type of show they watched.
