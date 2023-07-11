# Cryptocurrency Portfolio Proposal 

# Table of Contents
* [Background](#Background)
* [Files](#Files)
* [Instructions](#Instructions)
* [Analysis](#Analysis)
* [Conclusion](#Conclusion)


# Background
As an advisor in one of the top five financial advisory firms in the world, the objective is to propose a novel approach to assembling investment portfolios based on cryptocurrencies. The goal is to go beyond the traditional approach of solely considering returns and volatility, and include other factors that might impact the crypto market. By doing so, the aim is to create investment portfolios with better performance. The proposed approach involves clustering cryptocurrencies based on their performance in different time periods, using unsupervised learning techniques.

# Files
The following files are required for this project:

crypto_data.csv: Contains the price change data of cryptocurrencies in different periods.

# Instructions
The high-level steps for this challenge are as follows:

* Import the data and prepare it for analysis.
* Find the best value for k by using the original data.
* Cluster the cryptocurrencies with K-means using the original data.
* Optimize the clusters with Principal Component Analysis (PCA).
* Find the best value for k by using the PCA data.
* Cluster the cryptocurrencies with K-means using the PCA data.
* Visualize and compare the results.

# Analysis
Import and Prepare the Data
* The data is imported from the crypto_data.csv file and prepared for analysis. Summary statistics are generated, and the data is visualized using HvPlot.

Find the Best Value for k Using the Original Data
* The elbow method is implemented to find the best value for k in the range from 1 to 11. The inertia values are plotted, and the optimal value for k is determined.

Cluster the Cryptocurrencies with K-means Using the Original Data
* The K-means algorithm is applied to cluster the cryptocurrencies using the best value of k obtained from the original data. The clusters are predicted, and a scatter plot is created to visualize the clusters.

Optimize the Clusters with Principal Component Analysis
* Principal Component Analysis (PCA) is performed to reduce the features to three principal components. The explained variance is examined to determine the information attributed to each principal component. The total explained variance of the three principal components is calculated. A new DataFrame is created with the PCA data.

Find the Best Value for k Using the PCA Data
* The elbow method is applied using the PCA data to find the best value for k in the range from 1 to 11. The inertia values are plotted, and the best value for k is determined. It is compared to the best value obtained from the original data.

Cluster the Cryptocurrencies with K-means Using the PCA Data
* The K-means algorithm is used with the PCA data and the best value of k obtained from the PCA data to cluster the cryptocurrencies. The clusters are predicted, and a scatter plot is created to visualize the clusters.

Visualize and Compare the Results
* The cluster analysis results are visually analyzed and compared. Composite plots are created to contrast the elbow curves and the cryptocurrency clusters obtained from the original data and the PCA data.

# Conclusion
Based on the analysis and visualization of the cryptocurrency clustering using K-means and Principal Component Analysis (PCA), the following conclusions can be drawn:

* The best value for k using the elbow method with the original data is [best k value].
* Clustering the cryptocurrencies with K-means using the original data results in [number of clusters] clusters.
* Applying Principal Component Analysis (PCA) and reducing the features to three principal components explains [total explained variance] of the data.
* The best value for k using the PCA data is [best k value]. It differs from the best value obtained using the original data.
* Clustering the cryptocurrencies with K-means using the PCA data yields [number of clusters] clusters.
* Visual analysis shows that using fewer features with PCA affects the clustering results, leading to potential changes in cluster assignments.

For detailed analysis, code implementation, and visualizations, please refer to the Crypto_investments.ipynb Jupyter notebook for this project.

