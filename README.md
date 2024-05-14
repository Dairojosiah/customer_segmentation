# Customer Segmentation Analysis

## Project Overview


This repository contains a customer segmentation analysis performed using KMeans clustering, Principal Component Analysis (PCA), and Exploratory Data Analysis (EDA). The main goal of the analysis is to understand customer behavior and identify distinct customer segments to aid in targeted marketing strategies and business decision-making.

## Table of Contents
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Data Description](#data-description)
- [Methodology](#methodology)
  - [1. Exploratory Data Analysis (EDA)](#1-exploratory-data-analysis-eda)
  - [2. Principal Component Analysis (PCA)](#2-principal-component-analysis-pca)
  - [3. KMeans Clustering](#3-kmeans-clustering)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Structure

```
customer-segmentation/
│
├── data/
│   └── customer_data.csv
│
├── notebooks/
│   ├── EDA.ipynb
│   ├── PCA.ipynb
│   └── KMeans_Clustering.ipynb
│
├── src/
│   ├── data_preprocessing.py
│   ├── pca_analysis.py
│   └── kmeans_clustering.py
│
├── results/
│   └── cluster_visualizations.png
│
├── README.md
└── requirements.txt
```

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/customer-segmentation.git
    cd customer-segmentation
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Data Description

The dataset used in this analysis contains customer information with various features such as demographics and purchasing behavior. The data file is located in the `data/` directory.

## Methodology

### 1. Exploratory Data Analysis (EDA)

- **Objective:** Understand the structure and characteristics of the dataset.
- **Tasks:** Data cleaning, handling missing values, and visualizing data distributions.
- **Output:** Initial insights and potential features for clustering.

### 2. Principal Component Analysis (PCA)

- **Objective:** Reduce the dimensionality of the dataset while preserving variance.
- **Tasks:** Apply PCA to the standardized dataset and visualize the explained variance.
- **Output:** Reduced dimensional dataset ready for clustering.

### 3. KMeans Clustering

- **Objective:** Segment customers into distinct groups based on their behavior.
- **Tasks:** Determine the optimal number of clusters using the Elbow method, apply KMeans clustering, and interpret the results.
- **Output:** Identified customer segments and their characteristics.

## Results

The analysis identified distinct customer segments with unique characteristics. The results are visualized and saved in the `results/` directory. Key insights include:

- Number of clusters and their centroids.
- Characteristics of each customer segment.
- Visual representation of clusters in reduced dimensions.

## Usage

1. Run the EDA notebook:
    ```bash
    jupyter notebook notebooks/EDA.ipynb
    ```

2. Run the PCA analysis:
    ```bash
    jupyter notebook notebooks/PCA.ipynb
    ```

3. Run the KMeans clustering:
    ```bash
    jupyter notebook notebooks/KMeans_Clustering.ipynb
    ```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
