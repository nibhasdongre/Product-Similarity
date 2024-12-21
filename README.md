Product Similarity Search and Recommendation System
This repository contains a Product Similarity Search system developed for an e-commerce dataset. The system aims to identify and recommend products similar to a given product based on a combination of textual, numerical, and categorical features such as product name, price, rating, and discount.

Project Overview
The goal of this project was to build a model that ranks products based on their similarity to a given item. We utilized several similarity metrics to compute the distance between products:

TF-IDF for text-based similarity (product names)
MinMax scaling for numerical features (price, rating, etc.)
Jaccard similarity for categorical features (discount category, seller)
The final model combines these metrics to create a comprehensive similarity score for each product, which is then used for recommendation.

Key Features:
Text-based similarity: Using TF-IDF vectorization to compute cosine similarity based on product names.
Numerical similarity: Scaling numerical features and calculating Euclidean distance (inverted for similarity).
Categorical similarity: Using Jaccard similarity to compare categorical features like seller and discount category.
Customizable recommendations: The model allows you to retrieve the top-K most similar products for a given product.
Evaluation
The model's performance was evaluated using the following metrics:

Precision at K: Measures the proportion of recommended products that are relevant.
Recall at K: Measures the proportion of relevant products that are retrieved in the top-K recommendations.
F1 Score at K: A balanced measure combining precision and recall.
Results:
Precision at K: 0.6
Recall at K: 0.75
F1 Score at K: 0.67
These results indicate a good balance between recall and precision, with a slight focus on improving precision.
