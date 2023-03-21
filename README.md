# CryptoClustering-challenge
## Unsupervised Machine Learning 

For this project we'll use Python and Unsupervised Learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

The steps taken to get to the solution were as follows:
1. Prepare the Data
  - load crypto market data into a DataFrame
  - scale the data using StandardScaler from sklearn library
2. Find the Best Value for k Using the Original Scaled DataFrame
  - use a KMeans model
  - fit scaled data into model
  - extract inertia_ from model cluster
  - create an Elbow Curve with original data
3. Cluster Cryptocurrencies with K-means Using the Original Scaled Data
4. Optimize Clusters with Principal Component Analysis
5. Find the Best Value for k Using the PCA Data
6. Cluster Cryptocurrencies with K-means Using the PCA Data
7. Visualize and Compare the Results
