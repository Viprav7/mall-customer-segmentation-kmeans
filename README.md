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
3. **Model Training:** Trained the final K-Means model with 5 clusters using Scikit-Learn.
4. **Data Analysis:** Interpreted the clusters to discover 5 real-world customer personas (e.g., "Careless Spenders", "Frugal High-Earners", "VIPs").

##  Key Results
* Successfully isolated 5 clean, non-overlapping customer clusters.
* Provided actionable business insights on how to target different segments based on income-to-spending ratios.
