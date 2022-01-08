# Iterative K-means clustering on PySpark

![GoogleCloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-FFBA00?style=for-the-badge&logo=python&logoColor=white)

[![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/Naereen/StrapDown.js/blob/master/LICENSE)

This is the repository for the project  Iterative K-means clustering on PySpark. The idea behind K-Means algorithm is straightforward: in each iteration, k centroids are
initialized, each point in the space is assigned to the nearest centroid, and the centroids
are re-computed based on the assignment of points to clusters.

# Algorithm
![Alt text](https://raw.githubusercontent.com/aqid98/KMeans_PySpark/main/images/Kmean_Iterative.PNG?raw=true "Architecture")

# Data

The data contains 3 files:

(1) data.txt contains the vectorized version of documents, which has 4601 rows and
58 columns.

(2) c1.txt contains k initial cluster centroids. These centroids were chosen by
selecting k random points from the input data.

(3) c2.txt contains initial cluster centroids which are as far away as possible. You
could do this by choosing first centroid c1 randomly, and then finding the point c2
that is farthest from c1, then selecting c3 which is farthest from c1 and c2, and so
on.

