# Credit-card-Segmentation
Customer segmentation project using K-Means and Hierarchical Clustering on credit card data to identify distinct customer groups, evaluate clustering performance, and provide business insights.

## Project Goal 
To segment credit card customers into meaningful groups using unsupervised machine learning (K-Means and Hierarchical Clustering), helping a credit card company better understand customer behavior, improve marketing strategies, and enhance customer experience.

## Steps taken 
1. Data Preparation
-  Removed irrelevant columns (e.g., Customer ID).
-  Handled missing values (e.g., Defaulted).

2. Exploratory Data Analysis (EDA)
-  Explored feature distributions and correlations.
-  Identified spending patterns, outliers, and data trends.

3. Data Preprocessing
-  Standardized features using StandardScaler to ensure all features contributed equally to clustering.

4. K-Means Clustering
-  Used the Elbow Method → optimal clusters = 4.
-  Assigned each customer to a cluster.

5. Hierarchical Clustering
-  Built a dendrogram → cut at 5 clusters.
-  Assigned customers to clusters.

6. Evaluation
- Compared models with Silhouette Scores:
 - K-Means (k=4): 0.344 
 - Hierarchical (5 clusters): 0.244

## Findings

1. K-Means identified 4 distinct customer groups that could reflect:
 - High-value customers → high spenders with low default risk.
 - Moderate spenders → stable usage, medium engagement.
 - High-risk customers → higher likelihood of defaulting.
 - Low-activity customers → minimal spending and engagement.

2. Hierarchical clustering provided insights into customer similarity but did not produce as distinct clusters as K-Means.

## Recommendations 
- Targeted Marketing
  - Offer premium rewards and loyalty benefits to high-value customers.
  - Design engagement campaigns to encourage more activity from low-activity customers.
- Risk Management
  - Closely monitor high-risk customers.
  - Provide debt reduction or credit counseling programs to minimize defaults.
- Product Personalization
  - Create tiered credit card products that align with the needs of each customer cluster

## Next steps 
- Explore advanced clustering methods (DBSCAN, Gaussian Mixture Models).
- Combine clustering results with domain knowledge for richer interpretation.
- Track cluster behavior over time to monitor changes in customer segments.
