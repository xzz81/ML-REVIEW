# Description
A statistical techniques aimed at visualizing the similarity or dissimilarity ,model data as distance in a geometric space, often for visuulization in 2 ot 3 dimensions.

# Procedure
Begin with a matrix of dissimilarities between pairs of items. MDS find a set of vectors in a low-dimensional that approxiates these dissimilarities.

# Strength
Provide intuitive geometric representations of complex relationships amaong items, making it easier to identity patterns, clusters, or outliers within the data

# Limitation
It's sensitive to choice of dissimilarity and initial configuration. 
Hard to interpret.

# R command 
sim2diss(data, type = '') argument type dependent on the original data

cmdsacle(euromat, k = 2) #for distance

mds(crime.dist,ndim=2,type="interval") # for corr,rank, probability....
type = interval  # for metric, the diffrernce between data are meaningful, can be analiesd directly.
type = ordinal #just ordinal

