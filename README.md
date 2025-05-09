# Spare Parts Consumption Analysis and Clustering

This project analyzes the monthly consumption patterns of spare parts using Exploratory Data Analysis (EDA) and K-Means clustering.

## Objectives:

1.  Clean and prepare spare parts data.
2.  Explore consumption trends and variability.
3.  Identify high-variance months and materials.
4.  Cluster spare parts based on consumption patterns using K-Means.
5.  Visualize clusters using PCA.

## Data Description:

The data is stored in an Excel file and contains the monthly consumption of various spare parts. The key columns are:

* `Material`: Unique identifier for each spare part.
* `Jan` to `Dec`: Monthly consumption of the spare part.

## Methodology:

1.  **Data Loading and Preparation:**
    * The Excel file is loaded using pandas.
    * Missing values are filled with 0.
    * Duplicate materials are identified and dropped.

2.  **Exploratory Data Analysis (EDA):**
    * Descriptive statistics (mean, std, min, max, etc.) are calculated for each month's consumption.
    * Average monthly consumption is visualized using a bar plot to identify overall trends.

3.  **K-Means Clustering:**
    * K-Means clustering is applied to group spare parts based on their monthly consumption patterns.
    * The optimal number of clusters is determined using the Elbow Method.

4.  **Principal Component Analysis (PCA):**
    * PCA is used to reduce the dimensionality of the data to two principal components.
    * This allows for visualization of the clusters in a 2D scatter plot, making it     easier to understand the relationships between different consumption patterns.

## Results:

The analysis results in the identification of distinct clusters of spare parts, each representing a different monthly consumption pattern. These clusters can be described as:

* **Cluster 0:** Low and Steady Consumption
* **Cluster 1:** Seasonal Peak Consumption
* **Cluster 2:** High and Variable Consumption
* **Cluster 3:** Gradually Increasing/Decreasing Consumption

A bar chart of the average monthly consumption for each cluster is provided, enabling a clear visual comparison of the consumption patterns.  The clusters are also visualized using a 2D scatter plot of the first two principal components.

## Interpretation:

The clustering reveals significant differences in spare parts consumption patterns.  This information can be used to:

* Optimize inventory levels.
* Improve forecasting accuracy.
* Enhance warehouse efficiency.
* Reduce costs associated with spare parts inventory.
