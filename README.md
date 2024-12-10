# Text Classification of COVID-19 Related Tweets

## Project Overview

This project performs sentiment analysis on a dataset of tweets related to the COVID-19 pandemic using Natural Language Processing (NLP) techniques. The goal is to classify tweets into different sentiment categories using machine learning.

## Dataset

- Source: Corona_NLP_train.csv
- Total Tweets: 41,157
- Columns: UserName, ScreenName, Location, TweetAt, OriginalTweet, Sentiment

### Sentiment Distribution
- Positive: 11,422
- Negative: 9,917
- Neutral: 7,713
- Extremely Positive: 6,624
- Extremely Negative: 5,481

## Data Preprocessing
- Dropped unnecessary columns (username, screenname, location, tweet date)
- Used TF-IDF Vectorization for text feature extraction

## Machine Learning Model
- Algorithm: Linear Support Vector Classification (LinearSVC)
- Preprocessing Pipeline:
  1. TF-IDF Vectorization
  2. Linear SVC Classifier

## Model Performance
- Accuracy: 56.99%
- Confusion Matrix visualized to show classification performance across different sentiment categories

## Example Predictions
- Positive Tweet: "it is a warm, sunny, summer day" 
  - Predicted as: Positive
- Neutral-Positive Tweet: "the weather was nice but could have been much better"
  - Predicted as: Extremely Positive
- Negative Tweet: "it rained all day, i hated it!"
  - Predicted as: Extremely Negative

## Libraries Used
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Visualization Insights
- Top 5 Locations by Tweet Volume:
  1. London
  2. United States
  3. London, England
  4. New York, NY
  5. Washington, DC

## Future Improvements
- Experiment with more advanced NLP models
- Try ensemble methods
- Collect more diverse training data
- Implement more sophisticated text preprocessing

## How to Run
1. Install required libraries
2. Load the Corona_NLP_train.csv dataset
3. Run the Jupyter notebook/Python script

## Author
Melchizedek Ackah-Blay
Date: December 10, 2024
