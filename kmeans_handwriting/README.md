# K-Means Clustering - Handwriting Recognition 
This project uses k-means clustering to cluster images of handwritten numbers. This is how post offices, ATMs, etc also do handwriting recognition! 

NOTE: This project is based on Codecademy's [Handwriting Recognition project](https://www.codecademy.com/journeys/data-scientist-ml/paths/dsmlcj-22-machine-learning-i/tracks/dsmlcj-22-unsupervised-learning-algorithms-i/modules/mle-k-means-clustering-d0069e1f-bb75-469a-808e-68ff83284e40-155dbbbb-2ba8-42aa-90d2-a95b5983d2ae/projects/clustering). 


## Dataset
The dataset comes from `sklearn`. 

## Methods
1. Load in and look at datasets (incl. visualization of digits from pixel map)
1. Fit K-means model 
1. Visualize centroids as digits
1. Fit 2nd K-means model with a training and testing test, and use the model to predict new inputs

## Results and Discussion
Visually, the centroids as digits are fairly distinguishable, showing that the algorithm is appropriate and successful at this clustering task. The K-means model has a silhouette score of 0.163. As silhouette scores can range from -1:1, this is a bit low, showing that data points are not so well clustered. Considering the amount of variability in writing styles and the similarity of some digits, this makes sense. 

When training the 2nd model, it has a training silhouette score of 0.163, and a testing score of 0.160. When using it to predict new inputs, digit 9, it predicts that it belongs to cluster id 0, which looks like digit 9. Thus, even with a smaller training set, the model is accurate. 
