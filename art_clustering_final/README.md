## Machine Learning Assignment 3

Assignment: Work with a set of images of and metadata on ~400 works of fine art from museum collections and galleries **to cluster them on metadata and/or image characteristics**. 

Overview: I decided to work with the fine art clustering. I originally stuck with the original ordinal Bertin variables in the metadata but decided to add a few more. Since so many of the variables were Boolean variables, in Excel I did a find-and-replace on all Boolean True-False values to replace them with 0 and 1. The addition of these variables, I thought, would improve the groupings of the artworks. I also did this for spatial dimensions. 

After adding the features, I set to work on the k-means algorithm. The intertia / elbow plot showed an ideal clustering at around 12-15 clusters. I decided on 12 clusters, which did not result in a very high silhouette score, suggesting more work could be done on the features. However, I liked some of the clusters that were coming out of this group since they seemed to be grouping based on lines and edges. After some tinkering, I decided to stay with "init='random', n_init=200, max_iter=1000, tol=1e-10".

### [Silhouette1](https://github.com/mi-desai/msdv-ml-2020/tree/master/art_clustering_final/silhouette1.png)

### [Silhouette2](https://github.com/mi-desai/msdv-ml-2020/tree/master/art_clustering_final/silhouette2.PNG)

### [Silhouette3](https://github.com/mi-desai/msdv-ml-2020/tree/master/art_clustering_final/silhouette3.png)

### [Silhouette4](https://github.com/mi-desai/msdv-ml-2020/tree/master/art_clustering_final/silhouette4.PNG)


The results: 

### [Results](https://github.com/mi-desai/msdv-ml-2020/tree/master/art_clustering_final/results.png)
