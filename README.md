# Content-Based Recommendation System

A machine learning-based content recommendation system that recommends similar products based on their features. The system uses **cosine similarity** to identify similar products and provides an interactive recommendation interface using **Gradio**.

## 📌 Overview

This project implements a **Content-Based Recommendation System** using product-related features such as:

- Product brand
- Product rating
- Product price
- Customer/product interaction features
- Sentiment score
- Product category attributes

The system compares products based on their feature similarity and recommends products that are most similar to the selected product.

Products belonging to the **same brand as the selected product are excluded** from the recommendations.

## 🚀 Features

- Content-based product recommendation
- Data preprocessing and feature encoding
- Handling of missing values
- Feature scaling using Min-Max Scaling
- Product similarity calculation using Cosine Similarity
- Exclusion of products from the selected product's brand
- Selectable number of recommendations
- Interactive Gradio interface

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Gradio
- Jupyter Notebook

### Machine Learning Techniques

- One-Hot Encoding
- Min-Max Scaling
- Cosine Similarity

## ⚙️ How It Works

The recommendation system follows these steps:

1. **Load Dataset**
   - The product dataset is loaded using Pandas.

2. **Data Preprocessing**
   - Missing values are handled.
   - Categorical features are converted into numerical representations using One-Hot Encoding.

3. **Feature Selection**
   - Relevant numerical and categorical features are selected for recommendation.

4. **Feature Scaling**
   - Features are scaled using `MinMaxScaler` so that different feature ranges do not disproportionately affect similarity.

5. **Calculate Similarity**
   - Cosine Similarity is used to measure the similarity between products.

6. **Generate Recommendations**
   - The selected product is compared with other products.
   - Products are ranked based on similarity.
   - Products from the same brand are excluded.
   - Duplicate recommendations are removed.

7. **Display Recommendations**
   - The final recommendations are displayed through an interactive Gradio interface.

## 📂 Project Structure

```text
Content-Based-Recommendation-System/
│
├── Content Based Recommendation System.ipynb
├── content_based_recommendation_dataset.csv
└── README.md
