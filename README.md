# CryptoClustering

##Module 11 Challenge

###Description

Classify cryptocurrencies according to their price fluctuations across various time frames. Specifically, you will examine price changes over intervals spanning 24 hours, 7 days, 30 days, 60 days, 200 days, and 1 year.

####Implementation

- Import the data.
- Prepare the data by normalizing all columns.
- Find the best value of k (number of data clusters) by applying the Elbow Method on the original scaled data. We find that the Elbow Method suggests that k=4 is the best value.
- Apply the KMeans model to separate each crypto currency into one of the four clusters,
- Use a scatter plot to visualize the clusters.
- Use PCA to reduce the dimensionality of the data from 7 to 3.
- Calculate the variance of the original data that is captured by the three principal components.
- Use the Elbow Method on the PCA data to find the best value for k. It turns out that k=4 is again the best value.
- Apply the KMeans model to separate the PCA data into clusters.
- Use a scatter plot to visualize the PCA clusters and realize that they look very similar to the original clusters.
- Calculate the weights that each fluctuation timescale has on each principal component.

####Findings

- Using the elbow method on the original data and after PCA was applied, we find that both methods yield the same best value of four for the number of data clusters.

- We further see that using three principal components captures 89.5% of the variance of the original system whereas using only two principal components captures only 71.9% of the variance in the data. We therefore use three principal components.

- Visually comparing the clusters produced using the original data with the clusters produced after PCA shows that they are very similar, justifying the reduction of the dimensionality of the system from 7 to 3.

- Finally find that the different principal components capture the variances of different combinations of timescales.

####Sources

- Class Lessons
- Instructor
- Teacher Assistant
- Classmates
- Xpert Learning Assistant
