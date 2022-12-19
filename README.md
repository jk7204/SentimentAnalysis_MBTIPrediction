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
    - Determine the distribution of type of words: Nouns, Verbs, etc
- WordCloud
    - Determine words with the higher weights on each MBTI personality class
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
    - ![entj 4 32 29 PM](https://user-images.githubusercontent.com/100020447/208320877-8ed67a02-ce29-451f-8573-2444f47774c4.png) ENTJ
    - ![entj 4 09 12 PM](https://user-images.githubusercontent.com/100020447/208320881-6b3c4248-192b-418e-bc4e-612f5327daa6.png) ENTP
    - ![esfj 4 28 13 PM](https://user-images.githubusercontent.com/100020447/208320882-77292dbc-d6a0-44fc-945d-aa059dbb1875.png) ESTJ
    - ![enfj (1)](https://user-images.githubusercontent.com/100020447/208354930-0cac0942-2817-4568-b101-330fb73240f2.png) ENFJ
    - ![enfp](https://user-images.githubusercontent.com/100020447/208355142-e06041b7-6f50-4985-a6c8-93be69e301d8.png) ENFP
    - ![esfp](https://user-images.githubusercontent.com/100020447/208355161-df9933fa-639c-4531-9f7f-a2209ab1e073.png) ESFP
    - ![estj](https://user-images.githubusercontent.com/100020447/208355175-2f6c8821-13d2-41e0-8f4c-50daf6d3b4be.png) ESTJ
    - ![estp](https://user-images.githubusercontent.com/100020447/208355191-c4a2f068-6fba-4566-9c88-bf52c8811e5b.png) ESTP
    - ![infj](https://user-images.githubusercontent.com/100020447/208355204-98dd3c43-8dcb-4bae-9110-d1ebbfd6b70f.png) INFJ
    - ![infp](https://user-images.githubusercontent.com/100020447/208355216-fb93bcb8-d41c-4132-9e50-3221afa7b990.png) INFP
    - ![intj](https://user-images.githubusercontent.com/100020447/208355230-f781d3dd-f1f2-4e4e-82b1-574f834802b0.png) INTJ
    - ![intp](https://user-images.githubusercontent.com/100020447/208355244-f68fd8b4-5786-4244-9cf5-ac8c610e560c.png) INTP
    - ![isfj](https://user-images.githubusercontent.com/100020447/208355265-2684fa3b-11fe-4ba1-93ab-a5f565b750a9.png) ISFJ
    - ![isfp](https://user-images.githubusercontent.com/100020447/208355278-437567c4-5b5c-43e4-902c-c3a8a04d6fbf.png) ISFP 
    - ![istj](https://user-images.githubusercontent.com/100020447/208355291-01b09c5b-a35c-412b-9837-9236d530e1e3.png) ISTJ
    - ![istp](https://user-images.githubusercontent.com/100020447/208355310-9c4a5a90-8311-4f57-8334-6a97029b773d.png) ISTP





- Pie Chart
    - ![esfj](https://user-images.githubusercontent.com/100020447/208320992-2ab8fe7b-7e65-40df-8f04-a2d5fe4d8564.png) ESFJ
    - ![entp](https://user-images.githubusercontent.com/100020447/208321004-02fab3d8-2562-4b2e-964f-d2420cc54d01.png) ENTP
    - ![enfj](https://user-images.githubusercontent.com/100020447/208355585-456df028-d57d-41e2-9252-a26eb12ebb57.png) ENFJ
    - ![enfp](https://user-images.githubusercontent.com/100020447/208355600-fa764892-9ca7-42f3-8c26-aafcf30f8899.png) ENFP
    - ![entj](https://user-images.githubusercontent.com/100020447/208355619-b3d706d2-1678-4741-92f8-1fa4a7b78d3c.png) ENTJ
    - ![esfp](https://user-images.githubusercontent.com/100020447/208355638-3441031a-b9a6-485c-b04d-8968ac49c5a4.png) ESFP
    - ![estj](https://user-images.githubusercontent.com/100020447/208355654-0af94202-ee60-4995-9ec1-7f206fe2678c.png) ESTJ
    - ![estp](https://user-images.githubusercontent.com/100020447/208355667-e74b6c4e-7c7f-4695-b7e8-1ca93887ea8c.png) ESTP
    - ![infj](https://user-images.githubusercontent.com/100020447/208355678-17720a5d-3a72-4549-ab97-b5467a2213a5.png) INFJ
    - ![infp](https://user-images.githubusercontent.com/100020447/208355684-dfee9e57-50d5-4109-aa38-bcbb6b7b7b3d.png) INFP
    - ![intj](https://user-images.githubusercontent.com/100020447/208355687-487d4a82-284b-413f-834e-4708e968ada2.png) INTJ
    - ![intp](https://user-images.githubusercontent.com/100020447/208355709-a7d70377-207c-4f52-a5cd-48a04eb822f6.png) INTP
    - ![isfj](https://user-images.githubusercontent.com/100020447/208355722-f5fb2197-a412-4e39-b5de-a2da13d2957b.png) ISFJ
    - ![isfp](https://user-images.githubusercontent.com/100020447/208355734-22f29ec3-5314-4b19-8bc5-fece88395e9f.png) ISFP
    - ![istj](https://user-images.githubusercontent.com/100020447/208355770-843863f5-24a8-4026-bdc3-02c159c6510a.png) ISTJ
    - ![istp](https://user-images.githubusercontent.com/100020447/208355822-ec12c9a3-99bb-4166-95c5-fb91c7beba34.png). ISTP



- Accuracy Comparison
    - RNN: 59.4%
    - RNN with Attention: 59.7%
    - LSTM: 58%
    - LSTM with Attention:60.5%
    - GRU: 59.2%
    - GRU with Attention: 60.3%
    - BiLSTM: 59.8%
    - BiLSTM with Attention: 61.3%
- Best Model in terms of accuracy
    - Accuracy on training: BiLSTM
    - Accuracy on test: BiLSTM with Attention
- Improvement of performance with Attention Layer


# References
- https://www.16personalities.com/personality-types 
- https://www.kaggle.com/datasets/datasnaek/mbti-type 
- https://arxiv.org/pdf/2201.08717.pdf 
- https://ieeexplore.ieee.org/document/9578983 
- https://web.stanford.edu/class/archive/cs/cs224n/cs224n.1184/reports/6839354.pdf https://github.com/ianscottknight/Predicting-Myers-Briggs-Type-Indicator-with-Recurrent-Neura l-Networks (RNN and embedding layer) 
- https://github.com/udit19281/ML-Project (Naive Bayes & SVM) 
- https://medium.com/@dolly19304/personality-prediction-using-myers-briggs-type-indicator-568 88416e87c
- https://medium.com/geekculture/10-hyperparameters-to-keep-an-eye-on-for-your-lstm-model-and-other-tips-f0ff5b63fcd4
- https://medium.datadriveninvestor.com/attention-in-rnns-321fbcd64f05
