# A Data Analysis Project

## Overview

A comprehensive data analysis on the telecom customer churn dataset carried out as part of an interview process.

## Table of Contents

- [Requirements](#requirements)
- [Dataset](#dataset)
- [EDA](#eda)
- [Clustering](#clustering)
- [Predictive Model](#predictive-model)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Requirements

The dependencies or packages required for the project are specified in the requirements file.

    pip install -r requirements.txt

The entire process is carried out in notebook files (`.ipynb`).

## Dataset

- **Source**: [Link to the data source](https://www.kaggle.com/datasets/anshulmehtakaggl/cdrcall-details-record-predict-telco-churn)
- **Format**: CSV file.

## EDA (Exploratory Data Analysis)

Need to add in between comments

- **Data Head**: ![Data Head](images/df_head.png)
- **Data Info**: ![Data Info](images/df_info.png)
- **Descriptive Statistics**: ![Data Description](images/df_describe.png)
- **Inference**: ![Inference from statistical summary](images/describe_inference.png)
- **Handling NaN and Duplicates**: ![NaN and Duplicates](images/nan_duplicates.png)
- **Confirming Duplicates manually**: ![Locating dupes](images/loc_dupes.png)
- **Removing Duplicates**: ![Removing Duplicates](images/removing_dupes.png)
- **Box Plot After Removing Duplicates**: ![Box Plot After Removing Duplicates](images/box_plot_after_dupes.png)
- **Manual Outlier Check**: ![Manual Outlier Check](images/manual_outlier_check.png)
- **Addressing Outliers**: ![IQR function](images/iqr_fn_outlier.png)
- **Box Plot After Outlier Removal**: ![Box Plot After Outlier Removal](images/box_plot_after_outlier.png)
- **Histogram After Cleaning**: ![Histogram After Cleaning](images/hist_after_cleaning.png)
- **Correlation Heatmap**: ![Correlation Heatmap](images/corr_heatmap.png)

## Clustering

Need to add in between comments

- **Standardizing data before performing clustering**: ![Standardizing df](images/std_data.png)
- **Splitting df on 'Churn' feature**: ![Churn split](images/churn_split.png)
- **Clustering After Dimensionality Reduction**: ![Clustering After Dimensionality Reduction](images/cluster_then_dr.png)
- **Dimensionality Reduction then Clustering**: ![DR Then Cluster](images/dr_then_cluster.png)
- **Silhouette Score**: ![Silhouette Score](images/silhouette_score.png)
- **Optimized Clustering**: ![Optimized Clustering](images/optim_cluster.png)
- **K-Means vs Hierarchical Clustering**: ![K-Means vs Hierarchical Clustering](images/kmeans_vs_hierarchical.png)
- **K-Means Clustering Results on entire df**: ![K-Means Clustering Results](images/kmeans_entire_df.png)
- **Validating Churn rate in each cluster**: ![churn rate](images/validate_churn_rate.png)
- **K-Means Cluseting on Churn True**: ![K-Means Churn True](images/kmeans_churn_true.png)
- **K-Means Clustering on Churn False**: ![K-Means Churn False](images/kemeans_churn_false.png)

## Predictive Model

- **Predictive Models Overview**: ![Predictive Models Overview](images/predictive_models.png)
- **Saving Model**: ![Saving Model](images/saving_model.png)

## Usage

To be filled

## Contributing

TBF

## License

TBF

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
