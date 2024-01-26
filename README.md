# Shopping Recommender System README
## Overview
The Shopping Recommender System is designed to enhance the user experience in an e-commerce setting by providing personalized product recommendations to customers. The system employs a combination of collaborative filtering and content-based filtering techniques, with the integration of a hybrid model. This README provides an overview of the system's design, architecture, data preprocessing, visualization, recommendation techniques, evaluation metrics, and the benefits it offers to both the e-commerce organization and customers.

## Architecture
### 1. Data Preprocessing
The data preprocessing phase involves loading and cleaning transaction data from CSV files. Duplicate entries are removed, missing values are handled, and adjustments are made to 'Rate' and 'Qty' columns to ensure data accuracy.

### 2. Transactions Table Visualization
Exploratory data analysis is performed to gain insights into transaction data. Descriptive statistics, correlation matrices, and visualizations help understand product category distribution, quantity-rate relationships, and patterns based on store types.

### 3. Encoding and Standardization
Label encoding converts categorical variables like 'Store_type' into numerical representations. Date-related columns are standardized to datetime format, and a 'Net Sales' column is created for total net sales calculation.

### 4. Recommendation Techniques
### a. Content-Based Filtering
Utilizes TF-IDF vectorizer and cosine similarity to recommend products based on item characteristics. Evaluation metrics include precision, recall, F1 score, and mean average precision.

### b. Collaborative Filtering
Employs Singular Value Decomposition (SVD) to build a model based on user-item interactions. Evaluation metrics at the top-5 recommendations include precision, recall, F1 score, and mean average precision.

### c. Hybrid Filtering
Combines both content-based and collaborative filtering, weighting and combining recommendations from both models. Overall system performance is evaluated using precision, recall, F1 score, and mean average precision.

### 5. Evaluation Metrics
Crucial for assessing system performance, metrics differ for content-based, collaborative, and hybrid filtering. Metrics include average precision, recall, F1 score, precision@5, recall@5, F1 score@5, mean average precision@5.

### Evaluation Results
### Content-Based Filtering Metrics
**Average Precision**: 0.21
**Average Recall**: 0.0048
**Average F1 Score**: 0.0094
**Average Mean Average Precision**: 0.33
### Collaborative Filtering Metrics (Top-5 Recommendations)
**Precision@5**: 1.0
**Recall@5**: 1.0
**F1 Score@5**: 1.0
**Mean Average Precision@5**: 1.0
### Conclusion
The evaluation results highlight the exceptional performance of collaborative filtering, especially at the top-5 recommendations. Perfect precision, recall, F1 score, and mean average precision indicate highly accurate and relevant recommendations without false positives or negatives. Collaborative filtering emerges as the primary recommendation technique, emphasizing its effectiveness in capturing user preferences.

## Benefits
For E-commerce Organization and Customers
Customers: Enjoy personalized recommendations, enhancing shopping experience and product discovery.
Organization: Experience increased user engagement, higher conversion rates, improved customer satisfaction, and optimized product recommendations for targeted marketing efforts and increased sales.
**Note**: To improve the collaborative filtering model's performance, consider enriching the dataset with more diverse user-item interactions to ensure a broader representation of user preferences.






