Task 3: K-Means Clustering
Codveda Technologies Internship
Intern: Muhammad Sakibur Rahaman
Dataset: iris.csv

Objective
The objective of this task is to apply the K-Means clustering algorithm to the Iris dataset. We aim to group the Iris flowers into distinct clusters based on their sepal and petal measurements. This involves exploring the data, preprocessing it, determining the optimal number of clusters, applying the K-Means algorithm, and visualizing the results.

Steps Performed
Loaded and explored the dataset: The Iris dataset (iris.csv) containing 150 rows and 6 columns (Id, SepalLengthCm, SepalWidthCm, PetalLengthCm, PetalWidthCm, Species) was loaded and its basic properties were examined.

Feature Selection: The 'Id' column was dropped, and the four features ('SepalLengthCm', 'SepalWidthCm', 'PetalLengthCm', 'PetalWidthCm') were selected for clustering. The 'Species' column was kept aside for later comparison.

Feature Scaling: Numerical features were standardized using StandardScaler to ensure that all features contribute equally to the distance calculations in K-Means.

Determined Optimal Number of Clusters: The Elbow Method was used by calculating the Within-Cluster Sum of Squares (WCSS) for k values from 1 to 10. The "elbow" point was observed at k=3, indicating the optimal number of clusters.

Trained K-Means Model: The K-Means algorithm was applied with n_clusters=3 using the scaled features.

Visualized Clusters: The resulting clusters were visualized using scatter plots based on:

Sepal Length vs. Sepal Width

Petal Length vs. Petal Width

Compared with Actual Species: A contingency matrix (cross-tabulation) was created to compare the K-Means predicted clusters against the actual 'Species' labels to evaluate the clustering quality.

Repository Files
Task3_KMeans_Clustering_Iris.ipynb: Jupyter Notebook containing the complete Python code, step-by-step implementation, visualizations, and explanations.

README.md: This documentation file providing an overview of the task.

iris.csv: The dataset file used for this clustering task.

Results
✅ Dataset successfully loaded, explored, and preprocessed (features selected and scaled).

✅ The Elbow Method suggested k=3 as the optimal number of clusters, aligning with the known three Iris species.

✅ K-Means model was trained, and data points were successfully assigned to one of three clusters.

✅ Visualizations clearly showed distinct groupings of the Iris flowers, especially when using petal dimensions.

✅ Comparison with actual species labels via a contingency matrix showed that K-Means effectively separated Iris-setosa and provided a good (though not perfect) separation between Iris-versicolor and Iris-virginica.

Notes
K-Means clustering demonstrated its ability to uncover the inherent groupings within the Iris dataset without prior knowledge of the species.

The identified clusters largely correspond to the actual biological species, highlighting the effectiveness of the algorithm for this dataset.

Further evaluation could involve using other clustering metrics like the Silhouette Score.
