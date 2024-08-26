# A Data Analysis Project

## Overview

A comprehensive data analysis on the telecom customer churn [dataset](#dataset) carried out as part of an interview process.


Screenshots of the key steps were shown in the Sub-Headings, for the entire code with all the steps carried out do check out the jupyter notebook files.

## Table of Contents

- [Requirements](#requirements)
- [Dataset](#dataset)
- [Order of Procedure](#order-of-procedure)
- [Exploratory Data Analysis](#eda)
- [Clustering](#clustering)
- [Predictive Model](#predictive-model)
- [Contributing](#contributing)
- [License](#license)

## Requirements

The dependencies or packages required for the project are specified in the requirements file.

    pip install -r requirements.txt

The entire process is carried out in notebook files (`.ipynb`).

## Dataset

- **Source**: [Link to the data source](https://www.kaggle.com/datasets/anshulmehtakaggl/cdrcall-details-record-predict-telco-churn)
- **Format**: CSV file.
- Oh and it's also included in this repo itself.

## Order of Procedure
1. **Data Cleaning**: Begin by cleaning the data, removing any duplicates and outliers.
2. **Data Standardization**: Standardize the cleaned data to ensure consistency across all features.
3. **Dimensionality Reduction**: Perform dimensionality reduction (DR) on the standardized data to reduce complexity.
4. **Clustering**: Apply clustering techniques to the dimensionally reduced data for analysis.

## EDA

- **Data Head**: ![Data Head](images/df_head.png)
    - Taking a look at how the data is...
- **Data Info**: ![Data Info](images/df_info.png)
    - Checking the datatypes of the features present (Note:- Object is just string)
- **Descriptive Statistics**: ![Data Description](images/df_describe.png)
- **Inference**: ![Inference from statistical summary](images/describe_inference.png)
    - looking at the descriptive statistics these inference could be made
- **Handling NaN and Duplicates**: ![NaN and Duplicates](images/nan_duplicates.png)
    - Checking for Null/NaN values
- **Confirming Duplicates manually**: ![Locating dupes](images/loc_dupes.png)
    - Manually checking if the duplicates with the help of query function
- **Removing Duplicates**: ![Removing Duplicates](images/removing_dupes.png)
    - Addressing the duplicates by removing them
- **Box Plot After Removing Duplicates**: ![Box Plot After Removing Duplicates](images/box_plot_after_dupes.png)
    - Looking at the boxplot after removing dupes
- **Manual Outlier Check**: ![Manual Outlier Check](images/manual_outlier_check.png)
    - Investigating outliers for potentital impossible values
- **Addressing Outliers**: ![IQR function](images/iqr_fn_outlier.png)
    - Removing outliers with the help of iqr method (function as defined above) on the selected numerical features
- **Box Plot After Outlier Removal**: ![Box Plot After Outlier Removal](images/box_plot_after_outlier.png)
- **Histogram After Cleaning**: ![Histogram After Cleaning](images/hist_after_cleaning.png)
    - After addressing dupes & outliers looking at histogram for skewness in the distribution
- **Correlation Heatmap**: ![Correlation Heatmap](images/corr_heatmap.png)

## Clustering

Need to add in between comments

- **Standardizing data before performing clustering**: ![Standardizing df](images/std_data.png)
- **Splitting df on 'Churn' feature**: ![Churn split](images/churn_split.png)
- **Clustering then Dimensionality Reduction**: ![Clustering After Dimensionality Reduction](images/cluster_then_dr.png)
    - Performed clustering first before DR in hopes to find any complex cluster groups/patterns but all it ended up doing was take a lot of time to run nonetheless.
- **Dimensionality Reduction then Clustering**: ![DR Then Cluster](images/dr_then_cluster.png)
    - Optimal approach
- **Silhouette Score**: ![Silhouette Score](images/silhouette_score.png)
    - And so after seeing the different clustering choices from earlier, Hierarchical and KMeans seem to produce the best results. And so in order to find the optimal clusters I used the Silhouette score method.
- **Optimized Clustering**: ![Optimized Clustering](images/optim_cluster.png)
- **K-Means vs Hierarchical Clustering**: ![K-Means vs Hierarchical Clustering](images/kmeans_vs_hierarchical.png)
- **K-Means Clustering Results on entire df**: ![K-Means Clustering Results](images/kmeans_entire_df.png)
- **Validating Churn rate in each cluster**: ![churn rate](images/validate_churn_rate.png)
- **K-Means Cluseting on Churn True**: ![K-Means Churn True](images/kmeans_churn_true.png)
- **K-Means Clustering on Churn False**: ![K-Means Churn False](images/kemeans_churn_false.png)

## Predictive Model
### Building a predictive model on the entire df using ML algorithms for future steps
- **Predictive Models Overview**: ![Predictive Models Overview](images/predictive_models.png)
    - Didn't explore Neural Netowrks as the dataset size reduced to 36k from 110k ish after addressing dupes and outliers which could be easily handled by ML algs itself.
    - Above pic shows the models and their eval metrics.
- **Saving Model**: ![Saving Model](images/saving_model.png)

## Contributing

- As per the LICENSE feel free to use it and if you want to add on to this or rectify any mistakes I've made (I'm fairly new to this), you can do so by submitting a pull request. 

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
