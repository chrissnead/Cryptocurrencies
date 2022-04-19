# Cryptocurrencies

## Overview

The purpose of this analysis is to use unsupervised machine learning to provide a breakdown of cryptocurrency trading data and use the findings as new investment potential.

To successfully analyze the data, the below aspects are used to provide effective results: 
* **Data Preprocessing** (Selection, Transformation, Scaling) - the process of helping to prepare data for `Machine Learning` Algorithms.
* **Elbow Curve** - method to determine the best number of clusters needed for the algorithm to group the objects by.
* **Principal Component Analysis (`PCA`)** - statistical technique to speed up machine learning algorithms when the number of features is too high.
* **Clustering Algorithms (`KMeans`)** - the process of grouping similar objects/data points into clusters.
* **Visualization (`hvPlot`, `Plotly`)** - graphic libraries that allows us to create 2D and 3D graphs such as, scatter plots.

## Results

The original dataset contained 1,252 entries, however only 1,144 cryptocurrencies were currently trading. Null values were also removed from the dataset resulting in a total of 532 tradable cryptocurrencies.

![Crypto Table](Resources/Images/crypto-table.jpg)

The **Elbow Curve** method showed the slope at 4. This is the number of clusters that was used for the `KMeans` algorithm.

![Elbow Curve](Resources/Images/elbow-curve.jpg)

The clusters are plotted in a 3D scatter plot for visualization.

![3D Graph](Resources/Images/3d-graph.jpg)

## Resources
* Dataset from [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist)
* Software: Python 3.7.9, Anaconda 4.9.2 and Jupyter Notebooks 6.1.4
* Libraries: `Scikit-learn`, `Plotly`, `hvPlot`, `Pandas`
