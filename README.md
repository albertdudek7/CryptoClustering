# Crypto Clustering using K values and scaled DataFrame

Finding the best value for K for Original Scaled Data and PCA Data on several Crytpo Currencies.
By using the elbow method to identify best value for K. 

Get the summary statistics and plot the data to see what the data looks like before proceeding.

![image](https://github.com/albertdudek7/Crypto_Clustering_using_K_values/assets/127783844/b3bfc139-806f-40cb-b226-c61d96f07f5b)

Prepare the Data
Use the StandardScaler() module from scikit-learn to normalize the data from the CSV file.

![image](https://github.com/albertdudek7/Crypto_Clustering_using_K_values/assets/127783844/d4b501d1-fcf6-48f0-a6ec-c1d86bcac1af)


Find the Best Value for k Using the Original Scaled DataFrame

![image](https://github.com/albertdudek7/Crypto_Clustering_using_K_values/assets/127783844/4c6fa4af-4630-4f9a-8442-2797e1dfe72e)

![image](https://github.com/albertdudek7/Crypto_Clustering_using_K_values/assets/127783844/c322b6fe-7da8-42cd-80bf-a86a4bfd3274)

![image](https://github.com/albertdudek7/Crypto_Clustering_using_K_values/assets/127783844/cf84b718-445a-4bc9-8ff3-a16a033f06f8)



Find the Best Value for k Using the PCA Data

![image](https://github.com/albertdudek7/Crypto_Clustering_using_K_values/assets/127783844/29641a44-423e-402f-85da-52580953fb11)

Create a list with the number of k-values from 1 to 11.
Create an empty list to store the inertia values.
Create a for loop to compute the inertia with each possible value of k.
Create a dictionary with the data to plot the Elbow curve.
Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.
Answer the following question in your notebook:
What is the best value for k when using the PCA data?
Does it differ from the best k value found using the original data?
Cluster Cryptocurrencies with K-means Using the PCA Data
Use the following steps to cluster the cryptocurrencies for the best value for k on the PCA data:

Initialize the K-means model with the best value for k.
Fit the K-means model using the PCA data.
Predict the clusters to group the cryptocurrencies using the PCA data.
Create a copy of the DataFrame with the PCA data and add a new column to store the predicted clusters.
Create a scatter plot using hvPlot as follows:
Set the x-axis as "price_change_percentage_24h" and the y-axis as "price_change_percentage_7d".
Color the graph points with the labels found using K-means.
Add the "coin_id" column in the hover_cols parameter to identify the cryptocurrency represented by each data point.
Answer the following question:
What is the impact of using fewer features to cluster the data using K-Means?
