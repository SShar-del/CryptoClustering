# CryptoClustering

This project involves using the knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.


## Acknowledgements

 - Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.

## Features

### Data Loading

- Loaded the crypto_market_data.csv into a DataFrame and got the summary statistics and plotted the data.

### Data Preparation

- Used the StandardScaler() module to normalize the data from the CSV file and created a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

### Finding the Best Value for k Using the Scaled DataFrame

- Used the elbow method to find the best value for k and plotted the elbow curve in a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.
- Answered the question: What is the best value for k? 

### Clustered Cryptocurrencies with K-means Using the Scaled DataFrame

- Initialized the K-means model with the best value for k and fitted the K-means model using the scaled DataFrame. Predicted the clusters to group the cryptocurrencies using the scaled DataFrame.Created a copy of the scaled DataFrame and added a new column with the predicted clusters.
- Created a scatter plot using hvPlot as per given requirements.


### Optimize Clusters with Principal Component Analysis

- Used the original scaled DataFrame, performed a PCA and reduced the features to three principal components.

- Retrieved the explained variance to determine how much information can be attributed to each principal component and answered the question about the total explained variance of the three principal components.
- Created a new DataFrame with the scaled PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.


### Found the Best Value for k Using the PCA DataFrame

- Used the elbow method on the scaled PCA DataFrame to find the best value for k and plotted the elbow curve in a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.
- Answered the questions: What is the best value for k when using the scaled PCA DataFrame? Does it differ from the best k value found using the original scaled DataFrame?

### Clustered Cryptocurrencies with K-means Using the PCA DataFrame

- Initialized the K-means model with the best value for k and fitted the K-means model using the scaled PCA DataFrame. Predicted the clusters to group the cryptocurrencies using the scaled PCA DataFrame. Created a copy of the scaled PCA DataFrame and added a new column to store the predicted clusters.
- Created a scatter plot using hvPlot as per requirements.
- Answered the question: What is the impact of using fewer features to cluster the data using K-Means?
