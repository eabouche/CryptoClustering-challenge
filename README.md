# CryptoClustering-challenge
## Unsupervised Machine Learning 

This project uses Python and the Unsupervised Learning libraries to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

The steps taken to get to the solution were as follows:

### Prepare the Data 

1. load crypto market data into a DataFrame
2. scale the data using StandardScaler from the sklearn library

---
### Find the Best Value for k Using the Original Scaled DataFrame

3. use a KMeans model
4. fit scaled data into model
5. extract inertia_ from model cluster
6. create an Elbow Curve with original data to find right number of clusters

---
### Cluster Cryptocurrencies with K-means Using the Original Scaled Data

7. use right number of clusters (4) as input into KMeans model
8. predict the data clusters
9. create an hvplot scatter chart to display the new market clusters

---

### Optimize Clusters using Principal Component Analysis(PCA)

10. instantiate a PCA model with 3 components and "fit_transform" the scaled market dataframe into model
11. look at the explained_variance_ratio_
12. create a new dataframe for storing new PCA data
---
### Find the Best Value for k Using the PCA Data

13. use KMeans model with market pca dataframe
14. fit dataframe into KMeans model and capture the inertia_
15. display new pca elbow curve to find the best value for k: 4
---
### Cluster Cryptocurrencies with K-means Using the PCA Data

16. use KMeans with optimzed clusters per PCA Elbow Curve (4)
17. predict the pca data
18. plot the data using hvplot.scatter
---
### Visualize and Compare the Results
19. compare the 2 elbow curves from original scaled data vs pca data
20. compare the 2 scatter hvplots from original data vs pca data
21. determine which hvplot solution does a better job clustering the data into organized segments (answers in code file)
