# SentimentAnalysis_MBTIPrediction

## Project Description
In this era of modernization, every individual and company is utilizing the Myers-Briggs Type Indicator (MBTI) to determine the personality type of themselves or their current and future employees. Most state of the art Machine Learning tools and algorithms have not been deployed for MBTI personality types prediction and all research on MBTI personality types prediction from textual data, i.e. from social media posts is sparse. This contributes to our purpose of initiating this project which is identifying the best performing recurrent neural network on MBTI personality type prediction. 

In this project we will be focusing on the following:
- A sentiment analysis on the last 50 social media posts of every sampled individual in the data and the application of a weighting metric on the sentiment score accounting for which of the following categories: 
    - E (Extrovert) vs. I (Introvert)
    - S (Sensing) vs. N (Intuition)
    - T (Thinking) vs. F ( Feeling)
    - J (Judging) vs. P (Perceiving)
- The development and application of multiple RNN variant models to make predictions on MBTI personality types with the obtained results from the sentiment analysis.


## Content of Repository
Total of ... files:
- DataPrepocessing.ipynb: Tokenization, Word Lemmatization and Train-Test Split for the Kaggle Dataset
   - Kaggle Dataset: https://www.kaggle.com/datasets/datasnaek/mbti-type
- WordCloud & Pie Chart
- Hyperparameter Optimization with Hyperband
- RNN vs. RNN with Attention Layer
- LSTM vs. LSTM with Attention Layer
- GRU vs. GRU with Attention Layer
- BiLSTM vs. BiLSTM with Attention Layer


## Results
- Comparison of Accuracy 

