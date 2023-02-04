# Cryptocurrencies

## Overview

This is a very exciting project, as it involves Cryptocurrencies. Due to the huge popularity of Bitcoin, new investors are no longer convinced to invest in this currency as it has become unaffordable.

But just like bitcoin, there are many cryptocurrencies available on the market at affordable prices, and the idea of this project is to discover trends to convince Accountability Accounting, a prominent investment bank, that investing in these new currencies will pay off.

In this analysis we're going to use unsupervised Machine Learning models to analyse a cryptocurrency database and we're going to predict the number of clusters to obtain the results from our data.

## Results

To carry out this analysis we have  followed these steps:

1. Preprocessing the Data for PCA

To be able to perform PCA, we first preprocessed the dataset. We also used the get_dummies method to convert text features into indicator variables and we standardised the features with StandardScaler().

2. Reducing Data Dimensions Using PCA

We applied Principal Component Analysis (PCA) to reduce dimensions in our dataframe and created a new dataframe to hold the three principal components: PC 1, PC 2, PC 3

<img width="297" alt="Screenshot 2023-02-04 at 01 19 55" src="https://user-images.githubusercontent.com/112814924/216752464-aee7157a-83a0-4847-ae33-ff58b50350af.png">

3. Clustering Cryptocurrencies Using K-mean

In this step, we created an elbow curve to find the best value for k and according to the graph the best value for k is 4.

![elbow_curve](https://user-images.githubusercontent.com/112814924/216752709-5c0ac80b-6ab8-43e8-940c-0fcd3bab648b.png)

 We then applied the k-means algorithm to make predictions of the K clusters for our dataset.

4. Visualizing Cryptocurrencies Results

We create a 3D scatterplot to plot the clusters of our dataframe, and by hovering over each data point, we can see the CoinName and the Algorithm data.

https://user-images.githubusercontent.com/112814924/216735959-376c71b0-e765-4859-823e-fdf081a838a2.mov

To better visualize the data, we create a table where we can confirm that there are 532 tradable cryptocurrencies.

<img width="882" alt="Screenshot 2023-02-03 at 19 36 25" src="https://user-images.githubusercontent.com/112814924/216735974-17567b6f-4e07-4913-b2fb-dc87a0351402.png">

Another way to visualise our data is by creating a 2D scatterplot to find the relationship between TotalCoinsMined and TotalCoinSupply.

<img width="736" alt="Screenshot 2023-02-03 at 19 05 55" src="https://user-images.githubusercontent.com/112814924/216735981-4a74493e-2574-4377-893c-bfd24304d2aa.png">

## Summary

There are 532 tradable cryptocurrencies in total. The 3D graph allows us to better visualize the results since it is interactive and better shows the distribution of the 4 clusters.

### Resources
Data: crypto_data.csv
