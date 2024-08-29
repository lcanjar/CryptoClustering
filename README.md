# Module 11 Challenge
## UNC AI Bootcamp

# Assignment objective: to classify cryptocurrencies according to their pricing fluctaions using K-means alogorithm and PCA.

# Step 1 was to prepare the data using StandardScaler.
- Using the normalized data, create a dataframe and set index to 'coin_id'
- Validated results matched the data set showin the challenge

# Step 2 was to find the best K value (# of clusters)
- Created adn set k-value list (10) and inertia empty set
- In the k-loop, create model (random=2), fit model and append inertia_ value
- Created elbow_data dictionary with k and inertia values to plot the Elbow curve
- Create data frame and compared k and inertia values with challenge assignment; matched
- Ran the Elbow curve plot line and saw that 4 was the optimal clusters (k)

# Step 3 was to cluster the cryptocurrencies with K-means (4) using scaled data
- Created and fit the model
- Preducted clusters to group the scaled data
- Copied the dataframe and added "market_clusters" feature = predicted clusters
- Compared the output of the dataframe and graphed a scatter plot w/ x = 24h and y = 7d using the 'market_clusters' for c

# Step 4 was to optimize the clusters with PCA
- Created and fit the PCA model
- Total variance ratio to find the total explaned variance of the 3 PCA components
- Total was 89%
- Then created a new dataframe with PCA data, copied in the names from the original data as new feature ('coin_id), and reset index to 'coin_id'
- Using the same approach as Step 2, found the best value for k using PCA data: 4.   The same as the k value from the original data.

# Step 5 was to cluster the cyrptocurrencies with K-means using PCA data
- Used the same approach as step 3, but whith PCA data
- Then determined the weight of each feature on each PCA
- On PCA1, price_change_percentage_200d had the strongest (positive) influence.  
- On PCA2, price_change_percentage_30d had the strongest (positive) influence.  
- On PCA3, price_change_percentage_7d has the strongest (positive) influence.

___
Assignment completed by Louis Canjar
  
