# Customer Market Segmentation using K-Means Clustering

##  Project Overview
This project applies unsupervised machine learning to a retail dataset containing customer demographics and purchasing behavior. Using K-Means clustering, I successfully segmented the customer base into 5 distinct target personas, allowing marketing teams to design highly customized ad strategies.

##  Tech Stack & Libraries
* **Language:** Python
* **Environment:** Google Colab
* **Libraries:** Pandas, NumPy, Scikit-Learn (StandardScaler, KMeans), Seaborn, Matplotlib

## Methodology & Key Steps
1. **Data Preprocessing:** Dropped irrelevant features (`CustomerID`, `Gender`) and applied `StandardScaler` to ensure features like Age and Annual Income were on an equal scale for distance calculations.
2. **The Elbow Method:** Iterated through cluster sizes ($K = 1$ to $10$) and plotted inertia to identify the "elbow joint" at $K = 5$.
   <img width="2087" height="1407" alt="elbow_method_plot" src="https://github.com/user-attachments/assets/61977b0b-22f9-43e1-89df-fc6d99aa5418" />

4. **Model Training:** Trained the final K-Means model with 5 clusters using Scikit-Learn.
5. **Data Analysis:** Interpreted the clusters to discover 5 real-world customer personas (e.g., "Careless Spenders", "Frugal High-Earners", "VIPs").

##  Key Results
* Successfully isolated 5 clean, non-overlapping customer clusters.
* Provided actionable business insights on how to target different segments based on income-to-spending ratios.
<img width="3092" height="1658" alt="customer_clusters_plot" src="https://github.com/user-attachments/assets/b91e82c6-86b9-4b87-ac84-4c7acc124927" />

* Cluster 2 (Green - Top Left): "The Careless Spenders." Low income, but incredibly high spending scores. They buy everything in sight despite a tight budget.

* Cluster 1 (Orange - Top Right): "The Gold Mines / VIPs." High income AND high spending scores. These are the mall’s most valuable customers. Marketing teams target them aggressively with luxury rewards.

* Cluster 0 & 3 (Blue and Red - Center): "The Average Joes." They sit right in the middle for both income and spending. They represent the steady, predictable revenue baseline for standard stores.

* Cluster 4 (Purple - Bottom Right): "The Frugal High-Earners." High income, but incredibly low spending scores. They have deep pockets but choose to save their money. A marketing team would target these individuals with high-value discount coupons or loyalty incentives to get them to spend.
