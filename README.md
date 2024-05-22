# Customer-Segmentation-by-Income-and-Spending-Score

### Description:
This project implements K-Means clustering to segment customers into five distinct groups based on their annual income and spending score. 
The data is visualized in a scatter plot, where the x-axis represents annual income and the y-axis represents spending score. 
Different colors highlight the five identified clusters.
### Key Libraries:
•	Scikit-learn (for KMeans clustering)                                      
•	Matplotlib 
### Code Explanation:
The code utilizes the K-Means clustering algorithm from scikit-learn to group customers. Here's a breakdown of the key steps:
### 1.	Elbow Method for Optimal Cluster Selection (Optional):
-  The code iterates through a range of possible cluster numbers (e.g., 1 to 10) and calculates the Within-Cluster Sum of Squares (WCSS) for each iteration.  
-  The WCSS typically decreases as the number of clusters increases. The "elbow point" in the WCSS vs. number of clusters plot suggests the optimal number of clusters.  
- Note: You can include this section if you implemented the elbow method code. If not, remove this section.
###    2.	K-Means Model Creation:
-	A KMeans model is created with the chosen number of clusters (e.g., 5 in this case).
-	The k-means++ initialization method is used for selecting initial cluster centers, and random_state is set for reproducibility.
-	The model is trained on the customer data using the fit method.
###  3.	Cluster Label Prediction:
-	The fit_predict method is used to predict the cluster label for each data point based on the trained KMeans model.
-	These predicted cluster labels represent the customer segments.
### 4.	Data Visualization :
-	The code should visualize the data using a scatter plot.
-	The x-axis should represent income, the y-axis should represent spending score, and different colors should represent the five clusters identified by KMeans.

### Results and Insights:

 The scatter plot depicts customer distribution based on income and spending score. The K-Means algorithm has segmented them into five distinct clusters.
 Here are potential customer insights based on these segments:

### • High-Spenders (Cluster 1):
This cluster (potentially colored green) might represent customers with high income and high spending.
They are likely profitable and can be targeted for premium products or services.

### •	Low-Spenders (Cluster 2):
This cluster (potentially colored blue) might represent customers with low income and low spending. They might be more budget-conscious and can be targeted with value-oriented offerings.

### •	Mid-Range Customers (Clusters 3, 4, 5):
These clusters (potentially colored yellow, purple, and orange) represent customers with varying income and spending levels. Further analysis can help understand their specific needs and preferences.

By understanding these customer segments, businesses can develop more targeted marketing campaigns and refine their customer relationship management strategies.

### Running the Code:
1.	Install required libraries (e.g., pip install scikit-learn matplotlib or pip install scikit-learn seaborn).
2.	Replace the placeholder visualization code with your chosen library's implementation.
3.	Run the Python script.

### Further Exploration:
•	Experiment with different numbers of clusters to see how it affects the segmentation.
•	Explore other clustering algorithms for comparison.
•	Analyze the characteristics of each cluster in more detail.

