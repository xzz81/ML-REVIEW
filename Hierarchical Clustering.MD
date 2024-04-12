# Process
1.All observations start by being their own cluster  
2.calculate the dissimilarity between all the current clusters  
3.Merge the two clusters with the smallest dissimilarity into the cluster  
4.iterate steps 2 and 3 until there is one cluster  

# Distance metrics 
Euclidean distance  : the common distance  

Manhattan distance :
 $$d = |x_{1} -x_{2}| + |y_{1} - y_{2}|$$

 Consine similarity :
 $$ d =\frac{x_{1} \cdot x_{2}}{||x_{1}||\cdot||x_{2||}}$$


# Linkage function
## Complete linkage:  
the maximum distance between two clusters  

Dendrogram : channing, because it links elements are far apart, it has Short and Uniform Branches


## Single linkage:
the minimum distance between two clusters  
Dendrogram : crwoding , a point to one cluster can be closer to other cluster, it makes long chains and is likely to stairs

## Centroid linkage: 
the distance between 2 clusters will deterimend by the centorids  

Dendrogram : inversion ,Non-monotonicity ,meaning that the height at which clusters join does not necessarily increase as you move up the hierarchy(number of clusters increase, but the height don't)

tbc: ward's ,average linkage

# silhovfette plots
1. For one point in a specific cluster
$$S(i) = \frac{b_{i} - a_{i}}{max(a(i),b(i))}$$
$a_{i}$ is the avearge distance for $a_{i}$ with other points in this specific cluster  
$b_{i}$ is the avearge distance for $b_{i}$ with other points in the colsest cluster

Cluster Width: (its vertical[X] extension) reflects the number of data points it contains. Wider clusters indicate a larger number of data points.


Cluster Height: (its horizontal extension[Y]) shows the Silhouette values of these points. Higher average heights indicate better cluster quality because points are more tightly grouped within the cluster and more distantly related to points in other clusters.


Positive and Negative Values: Observe whether any data points have negative Silhouette values, indicating potential misclassification. If many points have Silhouette values close to or below 0, it might indicate that the clustering configuration needs adjustment.

Anyway, higer is better
