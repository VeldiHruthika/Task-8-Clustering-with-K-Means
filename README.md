Task 8: Clustering with K-Means

-Hey! This was my eighth task, where I worked on unsupervised learning using the K-Means algorithm to segment customers based on their behavior.

-I used the Mall Customer Segmentation dataset — which includes data like gender, age, annual income, and spending score of mall visitors.

What I did in this task:

1.Loaded the dataset and checked out the basic structure — including fields like Gender, Age, Income, and Spending Score.

2.Preprocessed the data:

i.Dropped the CustomerID column (not useful for clustering).

ii.Converted Gender to numeric format (Male = 0, Female = 1).

iii.Scaled the features using StandardScaler to bring everything to the same scale.

3.Used the Elbow Method to figure out the best number of clusters (K):

i.Tried different K values from 1 to 10.

ii.Plotted the inertia (within-cluster sum of squares).

iii.Picked K=5 based on the "elbow" in the curve.

4.Trained the KMeans model with optimal K (5) and got cluster labels for each customer.

5.Visualized the clusters:

i.Used PCA to reduce the data from multiple dimensions to just 2.

ii.Plotted a 2D scatterplot with colors showing different clusters.

6.Evaluated the clustering using Silhouette Score:

i.Score came out nicely around ~0.44–0.5 (good enough for unsupervised tasks).

ii.Helps in understanding how well-separated the clusters are.

