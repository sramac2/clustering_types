## Clustering Techniques Using DBSCAN and Hierarchical Clustering

Hierarchical clustering lets us choose the clusters manually by providing as params while DBSCAN discovers clusters depending on the density. Hierarchical does not handle noise occuring in the data but DBSCAN can detect and even label it appropriately. 

### Paramater Influence
Hierarchical
- n_clusters we provided determined how the clusters were formed and the final grouping. 
- We can use the dendogram to determine what would be the suitable and ideal cut 
- When data has a clear hierarchy, this type of clustering works well. 

DBSCAN
- the eps controls the neighborhood size. When its a small number, there will be more noise on the other hand, when its too large, clusters tend to merge
- min_samples we provided is used to determine what is the minimum points to form a dense region. 

### Pros and Cons
Hierarchical
- While this is easy to understand and visualize, it requires us to provide the cluster count manually. It might take effort to identify an optimum number. This is great for small to medium datasets. With large datasets, its much more expensive to perform the operation.
DBSCAN
- Since it has a noise detection built in, it can easily detect outliers. Also, it does not require specifying the clusters count. On the other hand, highly sensitive to eps and min_samples. When data density varies a lot, it can struggle. 


### Purpose 
To understand the two types of clustering technique: Hierarchical and DBSCAN and how different parameters within the techniques ends up in varying results. This can be used to determine clusters within the real world such as transportation routes for transportation company etc.

### Challenges
Understanding how the clustering works and the differences between the both. Plotting them based on different parameters and knowing what the different params like eps, and n_clusters meant and using them. 