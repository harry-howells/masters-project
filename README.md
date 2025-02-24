# masters-project
MSc Project using NLP and XGBoost to analyse customers of vegan/vegetarian food: 

The vegan/vegetarian food market is growing at a significant rate and reducing meat consumption is the most significant way an individual can reduce their environmental impact. The aim of the project was to use topic modelling and predictive analysis to improve understanding of vegan/vegetarian customer feedback to make recommendations to maximise the appeal and popularity of non-meat restaurants. The main objectives were to develop two topic models using different clustering algorithms to evaluate the impact of clustering algorithms on the performance of the topic models to establish how effective the BERTopic framework is in identifying topics from vegetarian/vegan food reviews.

This report evaluates the performance of two BERTopic models, one using Hierarchical Density-Based Spatial Clustering of Applications with Noise (HDBSCAN) and the other using K-means to extract findings from vegan/vegetarian food reviews. The models were evaluated using the accuracy of prediction of the rating of a restaurant review using XGBoost algorithm. 
Sentence Bidirectional Encoder Representations from Transformers (SBERT) was used to convert reviews into vector representations, followed by dimensionality reduction using Uniform Manifold Approximation and Projection (UMAP). 
For topic extraction, Count Vectorisation (CV) and Term Frequency-Inverse Document Frequency (TF IDF) were applied to clusters to identify semantically similar topics. Finally, XGBoost was used to predict ratings, utilising three features: the number of "cool," "funny," and "useful" upvotes for a review.
The analysis was performed on 120238 reviews from the Yelp dataset. The reviews used in analysis were only those that contained the string ‘veg’ in an attempt to remove reviews that were not discussing vegan or vegetarian topics.

The experimental analysis of both topic models predicted the rating of a review with an accuracy of 0.56 using XGBoost suggesting that changing the clustering algorithm had no impact on the quality of topics produced. The BERTopic framework effectively identified topics from vegan and vegetarian food reviews, achieving a CV coherence score of 0.55, which is a significant improvement compared to similar implementations. Both models also identified veganism and vegetarianism as two distinct topics implying that customers view the two diets as separately as cuisines from different countries. The literature review highlighted a significant disparity observed between the performance of the framework on non English languages. It is therefore recommended that the capabilities of the framework be tested on Spanish text as this is the second most spoken language on the internet in 2024.

This repository is made up of 3 programmes;
1) Data download, clean and pre-processing.
2) NLP and predictive analytics model using HDBSCAN.
3) NLP and predictive analytics model using K-means. 

