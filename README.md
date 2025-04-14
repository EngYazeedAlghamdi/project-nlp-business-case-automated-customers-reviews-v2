# 🛍️ Amazon Product Reviews & Clustering with Sentiment Analysis

## Project Overview

This project explores Amazon product reviews by performing:
- Sentiment classification (Positive, Neutral, Negative)
- Product clustering based on features
- Summarization of product reviews using Generative AI
- Data visualization for insights and recommendations

Our goal was to understand customer sentiments and cluster products into meaningful groups to help in better recommendations.

---

## Dataset

Source: Kaggle - Consumer Reviews of Amazon Products  
Files:
- `Datafiniti_Amazon_Consumer_Reviews_of_Amazon_Products.csv`
- `Datafiniti_Amazon_Consumer_Reviews_of_Amazon_Products_May19.csv`

Dataset contains:
- Product details (name, brand, category, etc.)
- Customer reviews and ratings
- Review metadata (username, helpful votes)

---

## Project Workflow

1. **Data Cleaning**
   - Removed duplicates and missing values
   - Cleaned text data (lowercasing, stripping spaces)

2. **Task 1: Sentiment Classification**
   - Transformed ratings into sentiment classes:
     - 1–2 ⭐: Negative
     - 3 ⭐: Neutral
     - 4–5 ⭐: Positive
   - Balanced the dataset for better training
   - Trained models (Logistic Regression, etc.)

3. **Task 2: Clustering**
   - Combined product details (name, categories, brand) into a single text field
   - Applied TF-IDF vectorization
   - Used KMeans clustering to form 5 clusters:
     - Cluster 0: Tablets
     - Cluster 1: Batteries
     - Cluster 2: Smart Home Devices
     - Cluster 3: Kindle Readers
     - Cluster 4: Kids Tablets
   - Visualized clusters using PCA and scatter plots

4. **Task 3: Review Summarization**
   - Used Generative AI (BART) to summarize top reviews per cluster
   - Highlighted top 3 products and worst product in each cluster
   - Displayed summaries directly in notebook output

5. **Visualizations**
   - Confusion matrix for sentiment classification
   - Pie chart for cluster distribution
   - Bar chart for average ratings per cluster

---

## Results

- **Sentiment Classification**
  - Accuracy: ~80%
  - Balanced sentiment distribution across classes
  - Model performed best on Positive and Neutral classes

- **Clustering**
  - Identified clear clusters of products
  - Insights into top and bottom products in each group

- **Summarization**
  - Generated concise summaries of product reviews
  - Provided actionable insights per product cluster

---

## Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Transformers (Hugging Face)
- Kaggle API

---

## Team

- 🧑‍💻 [Yazeed alghamdi]
- 📅 Date: April 2025




