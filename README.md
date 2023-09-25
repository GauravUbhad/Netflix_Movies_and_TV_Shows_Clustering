# Netflix_Movies_and_TV_Shows_Clustering

![image](https://github.com/GauravUbhad/Netflix_Movies_and_TV_Shows_Clustering/assets/143088895/c9c0e34a-9b7c-4b6e-81a7-9f0b26e390c9)


# Project Summary 

**Enhancing User Satisfaction and Reducing Churn through Comprehensive Analysis and Content-Based Recommendations on Netflix Dataset**

**Introduction**

The primary objective of this project is to leverage data analysis and machine learning techniques to enhance user satisfaction and reduce subscriber churn for Netflix, a leading streaming platform with over 220 million subscribers worldwide. The project utilizes a Netflix Dataset encompassing movies and TV shows up to the year 2019, sourced from Flixable. By categorizing and classifying these shows and films into distinct groups, we aim to create a seamless content recommendation system that caters to individual user preferences.

**Project Workflow:**

**1. Handling Null Values:**
The initial step in our project involves addressing missing data in the dataset. This ensures the integrity of our analysis and recommendations.

**2. Enhancing Data Organization:**
We refine and structure key details such as directors, actors, production locations, and content types to improve data presentation and analysis. This step ensures that the dataset is well-prepared for subsequent processing.

**3. Rating Categorization:**
Show ratings are restructured into meaningful categories such as "for adults," "for kids," "suitable for family viewing," and "unrated." This simplifies the understanding of content suitability for different user segments.

**4. Exploratory Data Analysis (EDA):**
Comprehensive EDA is conducted to unearth valuable insights within the dataset. By analyzing trends, patterns, and user preferences, we aim to identify areas for improvement in content recommendations and user engagement. EDA is a critical step in our strategy to reduce churn.

**5. Clustering with Text Data:**
To facilitate grouping of similar content, we tokenize, preprocess, and transform textual attributes such as director, cast, country, genre, rating, and description using the TF-IDF vectorizer. This text data is prepared for clustering.

**6. Dimensionality Reduction:**
To enhance the efficiency of our clustering algorithms, we employ Principal Component Analysis (PCA) to reduce the dimensionality of the dataset while preserving relevant information. This step optimizes the performance of subsequent clustering methods.

**7. Clustering Algorithms:**
Two clustering algorithms, K-Means Clustering and Agglomerative Hierarchical Clustering, are applied to the preprocessed data. The optimal number of clusters is determined through various evaluation methods, resulting in four clusters for K-Means and two clusters for hierarchical clustering. These clusters represent different content groups based on user preferences.

**8. Content-Based Recommender System:**
Leveraging a cosine similarity matrix, we develop a content-based recommender system. This system provides personalized content recommendations to users, taking into account their viewing history and preferences. By offering content that aligns with individual tastes, we aim to decrease subscriber churn and elevate user satisfaction.

**Conclusion:**
This comprehensive analysis and recommendation system are expected to significantly enhance user satisfaction on the Netflix platform. By providing tailored content recommendations and improving the understanding of user preferences through clustering and EDA, we anticipate a reduction in subscriber churn, one of Netflix's critical concerns. This strategic move aligns with Netflix's goal of retaining its vast user base and ensuring long-term success in the highly competitive streaming industry. As we continue to refine and optimize our recommendation system, we are confident that it will contribute to improved retention rates and increased user satisfaction for Netflix.


# Problem Statement

The core business problem that we aim to address is the need for Netflix, and similar streaming platforms, to adapt to the changing landscape of viewer preferences and content consumption patterns. Specifically, we seek to:

**1. Understand Viewer Preferences:** The first challenge is to gain a deep understanding of how viewer preferences have evolved over time. This includes identifying trends in content consumption, such as the shift from movies to TV shows, changes in genre popularity, and preferences for certain types of content based on demographics.


**2. Optimize Content Strategy:** With this understanding, Netflix needs to optimize its content acquisition and creation strategy. This involves decisions on which types of content to prioritize, whether to invest more in original series, how to balance the library between TV shows and movies, and which genres or themes are gaining traction among viewers.


**3. Evaluate Content Quality:** Beyond quantity, the quality of content is crucial. To ensure viewer satisfaction, Netflix needs to evaluate content quality using metrics like IMDb ratings and Rotten Tomatoes scores. This evaluation can help in identifying underperforming content that may need improvement or removal from the platform.


**4. Enhance Viewer Engagement:** By aligning content offerings with viewer preferences and quality expectations, Netflix aims to enhance viewer engagement. A more engaged user base is likely to result in increased subscriber retention, reduced churn, and potentially attracting new subscribers.


**5. Strategize Effectively:** Armed with insights into viewer preferences and content quality, decision-makers at Netflix can strategize effectively to ensure that viewer preferences remain at the heart of their content offerings. This includes making data-driven decisions on content acquisition, production, and recommendation algorithms.



# Variable Description

The variable description of the Netflix Movies and TV Shows Clustering Dataset is as follows:

1. **show_id**: Unique identifier for each movie/show.

2. **type**: Indicates whether the entry is a movie or a TV show.
3. **title**: Name of the movie or TV show.
4. **director**: Name of the director(s) of the movie or TV show.
5. **cast**: Names of the actors and actresses featured in the movie or TV show.
6. **country**: Country or countries where the movie or TV show was produced.
7. **date_added**: Date when the movie or TV show was added to Netflix.
8. **release_year**: Year when the movie or TV show was released.
9. **rating**: TV rating or movie rating of the movie or TV show.
10. **duration**: Length of the movie or TV show in minutes or seasons.
11. **listed_in**: Categories or genres of the movie or TV show.
12. **description**: Brief synopsis or summary of the movie or TV show.

# Conclusion

# Conclusions drawn from EDA


1. **Content Distribution:** Netflix's content library is divided approximately into two-thirds movies and one-third TV shows. This distribution suggests that while movies remain a significant part of the platform's offerings, TV shows have gained prominence over time.

2. **Audience Targeting:** Netflix caters to a diverse audience, with a significant amount of content targeted at adult and teen audiences. Family-friendly content, however, is more prevalent in the TV show category compared to movies. This highlights the platform's effort to appeal to a wide range of viewers.

3. **Role of Indian Actors:** Indian actors play a prominent role in Netflix movies, indicating the platform's recognition of the popularity of Indian cinema. However, it's noteworthy that popular Indian actors are notably absent from Netflix TV shows, suggesting potential for growth in this area.

4. **Prolific Directors:** The dataset reveals that Jan Suter is the most prolific director in the movie category, while Ken Burns leads in the TV show category on Netflix. This information can be valuable for understanding the influence of specific directors on content offerings.

5. **Content Production by Country:** The United States holds the top spot as the largest producer of both movies and TV shows on Netflix, followed closely by India. Japan and South Korea exhibit a higher proportion of TV shows compared to movies, indicating growth potential in this segment and the platform's commitment to international content.

6. **Popular Genres:** Among the genres available on Netflix, international movies, drama, and comedy are the most popular. This insight can guide content acquisition and production decisions to align with viewer preferences.

7. **Content Addition Patterns:** The analysis reveals that Netflix's content addition patterns have evolved over time. TV show additions have been on the rise since 2018, while movie additions have shown a decline. In 2020, there were fewer movie additions compared to 2019, but there was an increase in TV show additions. This trend underscores the platform's adaptation to changing viewer preferences.

8. **Peak Months for Additions:** For content additions, October, November, and December emerge as peak months for TV shows, while January, October, and November are favored for movie additions. February sees the least number of additions. These findings can inform the timing of content releases to maximize viewership.

9. **Addition Timing:** Both movies and TV shows tend to be added to Netflix at the beginning or middle of the month, with weekends being popular days for content additions. Understanding these timing patterns can help optimize content release schedules for viewer engagement.

10. **Content Duration:** Most movies on Netflix fall within the 80 to 120-minute range, indicating a preference for feature-length films. In contrast, TV shows typically have one or two seasons, suggesting that viewers engage with shorter episodic content.

# Conclusions drawn from ML Models


1. **Clustering Techniques Utilized:**
   In our analysis of the Netflix Movies and TV show dataset, we employed two clustering techniques: **K-Means Clustering** and **Agglomerative Hierarchical Clustering**. These techniques are fundamental in grouping similar data points, in our case, movies and TV shows, based on various attributes.

2. **Optimal Number of Clusters:**
   - For K-Means Clustering, we determined that the optimal number of clusters for the dataset is 4. This means that the dataset can be naturally divided into four distinct groups or clusters based on the chosen attributes.
   - In contrast, Agglomerative Hierarchical Clustering yielded an optimal number of clusters of 2. This suggests that, from a hierarchical perspective, the dataset can be grouped into two major categories.

3. **Choice of Evaluation Metric - Silhouette Score:**
   In the process of evaluating the clustering results, we opted for the **Silhouette Score** as our preferred metric. The Silhouette Score is chosen over the distortion score for several reasons:
   - The Silhouette Score provides a more intuitive and easily interpretable result. It measures the quality of clusters by assessing the distance between data points within the same cluster and the distance between data points in different clusters.
   - It is less influenced by the shape of the clusters, making it a robust choice for our analysis. This means that it can handle clusters of varying shapes and sizes effectively.

**Recommendation System Development:**

1. **Motivation for Recommendation System:**
   We developed a recommendation system with the primary goal of enhancing the user experience and reducing subscriber churn for Netflix. Subscriber churn, or the rate at which subscribers cancel their subscriptions, is a critical concern for streaming platforms. To address this, we aimed to provide users with content recommendations that align closely with their individual preferences.

2. **Personalized Recommendations:**
   The recommendation system we developed offers personalized recommendations to users. It does so by calculating similarity scores between users and content. This personalized approach ensures that subscribers receive content suggestions tailored to their specific tastes and viewing history.

3. **Reducing Subscriber Churn:**
   By delivering content recommendations that are more aligned with user preferences, we aim to enhance user satisfaction and engagement with the platform. When users find content that resonates with them, they are more likely to continue their subscriptions and stay engaged with the platform. This, in turn, contributes to a reduction in subscriber churn, which is a critical metric for the long-term success of Netflix and similar streaming services.


