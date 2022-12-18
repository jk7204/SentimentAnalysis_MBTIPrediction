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

## Content of repository:
### Total of 1 files consisting of：
- DataPrepocessing: 
    - Data Cleaning: Removing unnecessary words and symbols
    - Word Lemmatization: Tokenize and lemmatize words to original form 
    - Distribution Identification: Draw distribution data for each MBTI personality class
    - Train-Validation-Test Split on Dataset: Training-75%, Validation-15%, Test-15%
    - Bag of Words Techniques
    - Kaggle Dataset: https://www.kaggle.com/datasets/datasnaek/mbti-type
- PieChart
    - Determine the distribution of type of words: Nouns, Verbs, etc.
    - ![esfj](https://user-images.githubusercontent.com/100020447/208320992-2ab8fe7b-7e65-40df-8f04-a2d5fe4d8564.png) ESFJ
    - ![entp](https://user-images.githubusercontent.com/100020447/208321004-02fab3d8-2562-4b2e-964f-d2420cc54d01.png)ENTP

- WordCloud
    - Determine words with the higher weights on each MBTI personality class
    - ![entj 4 32 29 PM](https://user-images.githubusercontent.com/100020447/208320877-8ed67a02-ce29-451f-8573-2444f47774c4.png) ENTJ
    - ![entj 4 09 12 PM](https://user-images.githubusercontent.com/100020447/208320881-6b3c4248-192b-418e-bc4e-612f5327daa6.png) ENTP
    - ![esfj 4 28 13 PM](https://user-images.githubusercontent.com/100020447/208320882-77292dbc-d6a0-44fc-945d-aa059dbb1875.png) ESTJ


- Hyperparameter Optimization with Hyperband
    - Determine the best configurations of number of hidden units, batch size, dropout, and learning rate for RNN, LSTM, GRU and BiLSTM models to enable best accuracy
    - HyperbandScheduler()
- RNN vs. RNN with Attention Layer
    - Build RNN and RNN with Attention Layer with the configurations with best accuracy obtained from running hyperband
    - Compare the performance of both models and determine if there exist improvement after adding Attention Layer
- LSTM vs. LSTM with Attention Layer
    - Build LSTM and LSTM with Attention Layer with the configurations with best accuracy obtained from running hyperband
    - Compare the performance of both models and determine if there exist improvement after adding Attention Layer
- GRU vs. GRU with Attention Layer
    - Build GRU and GRU with Attention Layer with the configurations with best accuracy obtained from running hyperband
    - Compare the performance of both models and determine if there exist improvement after adding Attention Layer
- BiLSTM vs. BiLSTM with Attention Layer
    - Build BiLSTM and BiLSTM with Attention Layer with the configurations with best accuracy obtained from running hyperband
    - Compare the performance of both models and determine if there exist improvement after adding Attention Layer
- Comparison of models and model variants with Attention Layer
    - Model with Best Accuracy
    - Performance improvement with Attention Layer

## Result
- WordCloud
- Pie Chart
- Accuracy Comparison
- Best Model
- Test on Trump Data??


