# YouTube Trend Analysis and Viral Video Prediction

## Overview

This project analyzes YouTube trending video data and uses machine learning models to predict whether a video will become viral based on engagement metrics such as likes, dislikes, comments, and publishing time.

## Dataset

* Dataset: YouTube Trending Videos Dataset
* Source: Kaggle
* Country Used: India (INvideos.csv)
* Total Records: 37,352 videos

## Objectives

* Perform exploratory data analysis (EDA) on YouTube trending videos.
* Identify relationships between views and engagement metrics.
* Create a viral video classification target.
* Train and evaluate multiple machine learning models.
* Determine the most important factors influencing video virality.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* KaggleHub
* Google Colab

## Data Preprocessing

* Removed missing values.
* Converted publish_time to datetime format.
* Extracted:

  * Publish Hour
  * Publish Day
* Created a viral label using the 75th percentile of views as the threshold.

## Exploratory Data Analysis

The project includes:

* Distribution of video views
* Top video categories
* Views vs Likes scatter plot
* Correlation heatmap
* Feature importance visualization

## Features Used

* Likes
* Dislikes
* Comment Count
* Publish Hour
* Publish Day

## Machine Learning Models

### Logistic Regression

Accuracy: 87.36%

### Decision Tree

Accuracy: 91.66%

### Random Forest

Accuracy: 94.24%

## Model Performance

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 87.36%   |
| Decision Tree       | 91.66%   |
| Random Forest       | 94.24%   |

Random Forest achieved the highest accuracy and was selected as the best-performing model.

## Feature Importance

| Feature       | Importance |
| ------------- | ---------- |
| Dislikes      | 0.4068     |
| Likes         | 0.2922     |
| Comment Count | 0.1857     |
| Publish Hour  | 0.0739     |
| Publish Day   | 0.0414     |

The results indicate that engagement metrics are the strongest predictors of video virality.

## Results

* Random Forest outperformed all other models.
* Likes, dislikes, and comment count were the most influential features.
* Publishing time had a smaller impact on predicting virality.

## Future Improvements

* Include title and description sentiment analysis.
* Use Natural Language Processing (NLP) on video metadata.
* Experiment with XGBoost and LightGBM.
* Build a web dashboard for real-time predictions.

## Author

Anurag pratap
