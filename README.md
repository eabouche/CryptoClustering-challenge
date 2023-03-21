# CryptoClustering-challenge
## Unsupervised Machine Learning 

For this project we'll use Python and Unsupervised Learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

The steps taken to get to the solution were as follows:
### Prepare the Data 
1 load crypto market data into a DataFrame
2 scale the data using StandardScaler from sklearn library

---
### Find the Best Value for k Using the Original Scaled DataFrame
3 use a KMeans model
4 fit scaled data into model
5 extract inertia_ from model cluster
6 create an Elbow Curve with original data to find right number of clusters

---
3. Cluster Cryptocurrencies with K-means Using the Original Scaled Data
3.1 use right number of clusters (4) as input into KMeans model
3.2 predict the data clustered
3.3 create an hvplot scatter chart to display the market clusters
-
5. Optimize Clusters with Principal Component Analysis
6. Find the Best Value for k Using the PCA Data
7. Cluster Cryptocurrencies with K-means Using the PCA Data
8. Visualize and Compare the Results
