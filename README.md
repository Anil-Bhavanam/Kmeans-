# Kmeans-

# init_centroids(K_Value, data_value):

This function initializes the centroids for the k-means clustering algorithm.
It takes two parameters: K_Value (the number of clusters) and data_value (the data points).
It randomly selects K_Value centroids within the range of the data points in each dimension (x and y).
The centroids are stored in a list and returned as a numpy array.
# dist(a, b):

This function calculates the Euclidean distance between two points a and b.
It takes two parameters: a and b (two points represented as arrays).
It computes the square root of the sum of squared differences between corresponding elements in a and b.
The distance value is returned.
# assign_cluster(K_Value, data_value, cg):

This function assigns each data point to its closest centroid.
It takes three parameters: K_Value (the number of clusters), data_value (the data points), and cg (the current centroids).
It iterates over each data point and calculates the distance to each centroid.
The data point is assigned to the cluster with the closest centroid.
The function returns an array representing the cluster assignments for each data point.
# compute_centroids(K_Value, data_value, cluster):

This function computes the new centroids based on the current cluster assignments.
It takes three parameters: K_Value (the number of clusters), data_value (the data points), and cluster (the current cluster assignments).
It iterates over each cluster and calculates the mean of the data points assigned to that cluster.
The mean values are stored in a list and returned as a numpy array.
# measure_change(cg_prev, cg_new):

This function measures the change in centroids between two iterations.
It takes two parameters: cg_prev (the centroids from the previous iteration) and cg_new (the updated centroids).
It iterates over each pair of corresponding centroids and calculates the distance between them.
The sum of the distances is returned as a measure of the overall change in centroids.
#show_clusters(data_value, cluster, cg):

This function visualizes the clusters and centroids using a scatter plot.
It takes three parameters: data_value (the data points), cluster (the cluster assignments), and cg (the centroids).
It creates a pandas DataFrame with columns 'x', 'y', and 'label' representing the data points and their cluster assignments.
The data points are plotted as scatter points with different colors for each cluster.
The centroids are plotted as stars.
The scatter plot is displayed using matplotlib.

Overall, these functions provide the necessary components for performing the k-means clustering algorithm, including centroid initialization, distance calculation, cluster assignment, centroid update, convergence measurement, and visualization of the clusters.
