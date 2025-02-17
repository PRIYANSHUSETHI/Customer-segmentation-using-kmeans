# Customer Segmentation using K-Means Clustering

## Overview
This project applies K-Means clustering to segment customers based on spending behavior. The dataset used is `Mall_Customers.csv`, which contains customer demographic and spending data. The project aims to categorize customers into distinct groups for targeted marketing strategies.

## Dataset
The dataset consists of the following columns:
- **CustomerID**: Unique identifier for each customer
- **Gender**: Gender of the customer
- **Age**: Age of the customer
- **Annual Income (k$)**: Annual income in thousands of dollars
- **Spending Score (1-100)**: Score assigned based on customer spending behavior

## Libraries Used
The following Python libraries are utilized:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `sklearn.cluster`

## Project Workflow
### 1. Data Loading and Exploration
- The dataset is loaded using pandas.
- A preview of the dataset is displayed using `.head()`.
- The shape, data types, and missing values are checked.

### 2. Selecting Features for Clustering
- The segmentation is performed using **Annual Income** and **Spending Score**.
- These features are extracted into a NumPy array for clustering.

### 3. Finding Optimal Number of Clusters
- The **Elbow Method** is used to determine the optimal number of clusters.
- Within-Cluster Sum of Squares (WCSS) is computed for different cluster sizes (1-10).
- A line plot is generated to visualize the elbow point.

### 4. Applying K-Means Clustering
- K-Means is initialized with the optimal number of clusters (determined from the elbow graph).
- The model is trained, and each data point is assigned to a cluster.

### 5. Visualizing Clusters
- The identified clusters are plotted using `matplotlib`.
- Different colors represent different clusters, and centroids are marked.

## Results
- Customers are grouped into five clusters based on their income and spending behavior.
- This segmentation helps in understanding different customer types, such as **big spenders**, **low spenders**, and **moderate customers**.

## Future Improvements
- Include additional features such as **age** and **gender** for better segmentation.
- Explore other clustering algorithms like **DBSCAN** or **Agglomerative Clustering**.
- Implement automated customer labeling based on segmentation insights.

## Conclusion
This project successfully segments customers using K-Means clustering, providing valuable insights into customer behavior. The methodology can be extended for various industries like retail, banking, and e-commerce for improved customer targeting strategies.
