# 🛍️ Product Recommendation System with Review-Based Sentiment Analysis
This project aims to build a content-based product recommendation system using review summaries and sentiment scores. It leverages Natural Language Processing (NLP) and machine learning to suggest the top 5 similar products based on review content and user ratings.

🎯 Objectives
Analyze product reviews from the Home & Kitchen category (Amazon 5-core dataset)

Preprocess and transform review text for feature extraction

Apply TF-IDF vectorization for NLP-based modeling

Use K-Nearest Neighbors (KNN) to recommend similar products

Visualize review sentiment using word clouds

📦 Dataset
Amazon Home and Kitchen 5-core reviews

Contains: reviewerID, asin, reviewText, overall rating, summary, reviewTime, etc.

Filtered to products with >100 reviews for quality modeling

🧪 Key Components
Text Cleaning: Lowercasing, punctuation removal, and stopword filtering

Feature Extraction: TF-IDF vectorization on summary_review text

KNN Classification: Predict review ratings and find nearest neighbors for product recommendation

Evaluation: Accuracy = ~89.5%, MSE = ~0.105

Visualization: Word clouds for each rating group to explore sentiment distribution

🔧 Tech Stack
Language: Python

Libraries: pandas, numpy, scikit-learn, matplotlib, wordcloud, re, json

Model: KNeighborsClassifier, NearestNeighbors (distance-weighted KNN)

NLP Tools: TfidfVectorizer (with bigrams and max_features=500)

📊 Results
Accurately predicted product ratings using review text

Generated top-5 product recommendations for selected items

Revealed key sentiment patterns through word clouds

📁 Project Structure
product_recommender_.ipynb: Full notebook with code, preprocessing, modeling, and visualizations

Word cloud plots for visual sentiment analysis

KNN implementation for both rating prediction and product similarity

