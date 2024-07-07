Cryptocurrency Market Analysis with Clustering
Overview
This project utilizes machine learning techniques to analyze and cluster cryptocurrency market data. The main steps include data preprocessing, clustering with K-means, and dimensionality reduction using PCA.

Project Structure
Data Source: Cryptocurrency market data is loaded from a CSV file (crypto_market_data.csv).
Libraries Used:
pandas: Data manipulation and analysis.
hvplot.pandas: Interactive plotting.
sklearn: Machine learning models including KMeans, PCA, and StandardScaler.
Project Workflow
1. Data Loading and Preprocessing
The cryptocurrency market data is loaded into a Pandas DataFrame (df_market_data).
Summary statistics and initial data visualization using hvplot are performed to understand the data.
2. Data Preparation
The data is standardized using StandardScaler to normalize numerical features.
A new DataFrame (df_market_data_scaled) is created with the scaled data.
3. Clustering with K-means
Finding the Optimal k:

The Elbow method is employed to determine the optimal number of clusters (k).
Inertia values for different values of k are computed and plotted to find the elbow point.
Clustering:

K-means clustering is applied with the optimal k value obtained from the elbow method.
Cryptocurrencies are grouped into clusters based on their scaled features.
4. Visualization
Scatter plots using hvplot.scatter visualize clusters based on selected features.
Cryptocurrency names are included in the hover information for easy identification.
5. Dimensionality Reduction with PCA
Principal Component Analysis (PCA) is applied to reduce the dimensionality of the data while retaining important features.
The explained variance of principal components is calculated to assess information retention.
6. Optimizing Clusters with PCA
Similar to the original data, the optimal k value is determined using PCA-transformed data.
K-means clustering is applied to the PCA-transformed data to optimize clusters.
Files Included
crypto_market_data.csv: Raw data file containing cryptocurrency market data.
crypto_analysis.ipynb: Jupyter Notebook containing the Python code for data analysis and clustering.
Requirements
Python 3.x
Pandas
hvPlot
scikit-learn
Instructions
Clone the repository to your local machine.
Install the required libraries using pip install -r requirements.txt.
Open crypto_analysis.ipynb in a Jupyter Notebook environment.
Run each cell in the notebook sequentially to replicate the analysis and visualization.
Conclusion
This project demonstrates how machine learning techniques can be used to analyze and cluster cryptocurrency market data. By applying K-means clustering and PCA, insights into the structure of cryptocurrency movements can be gained, aiding in investment decisions and market analysis.
