# COVID-19 Data Clustering using K-Means and MiniBatch K-Means

## Overview
This project analyzes COVID-19 data in Indonesia using clustering techniques. The dataset is processed, cleaned, and analyzed before applying K-Means and MiniBatch K-Means clustering algorithms to group provinces based on total cases, recovered cases, and deaths.

## Dataset
- The dataset is sourced from Google Drive and loaded using Pandas.
- The data consists of COVID-19 records for different provinces in Indonesia.
- The dataset is preprocessed by removing extra spaces in column names, converting the date column to datetime format, and handling missing values.

## Preprocessing Steps
1. Load dataset from Google Drive.
2. Standardize column names by converting them to lowercase and replacing spaces with underscores.
3. Remove columns with missing values.
4. Convert the `date` column to `datetime64` format.

## Data Analysis
- Compute total cases, deaths, and recoveries per province.
- Calculate active cases, death percentage, and recovery percentage.
- Identify correlations between features.
- Visualize the data using bar charts to show trends across provinces.

## Clustering Methods
### K-Means Clustering
- Performed clustering using the K-Means algorithm.
- Evaluated clusters using:
  - **Silhouette Score**: Measures cluster cohesion and separation.
  - **Davies-Bouldin Index (DBI)**: Evaluates clustering compactness and separation.
  - **Elbow Method**: Determines the optimal number of clusters based on inertia.

### MiniBatch K-Means Clustering
- Implemented MiniBatch K-Means for efficient clustering on large datasets.
- Used the same evaluation metrics as standard K-Means.

## Results
- Silhouette Score and Davies-Bouldin Index help determine the optimal number of clusters.
- The Elbow Method visualizes the best number of clusters by analyzing inertia values.
- Clustering results help understand COVID-19 distribution patterns across Indonesian provinces.

## Visualization
- **Total cases per province** (bar chart)
- **Top 10 provinces with the highest death percentage** (bar chart)
- **Cluster evaluation using Silhouette Score and DBI** (line plots)
- **Elbow Method for optimal k determination** (line plot)

## Requirements
- Python 3.x
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `sklearn`

## How to Run
1. Mount Google Drive to access the dataset.
2. Run the preprocessing and analysis steps.
3. Execute K-Means and MiniBatch K-Means clustering.
4. Evaluate and visualize results.

## Conclusion
This project provides insights into COVID-19 trends in Indonesia by clustering provinces based on key metrics. The analysis helps understand patterns of infection, recovery, and mortality across different regions.

