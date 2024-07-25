# Video-Transcribing-Sentiment-Analysis
Transcribing a video and performing Sentiment Analysis

In this project we have a Review Video called "Review.mp4" which we have to work with. These are our 2 objectives:
- Transribe the video
- Perform sentiment analysis on this text to detect the change in sentiments over time

Install the follwing libraries before running the Python script:
- moviepy
- pydub
- SpeechRecognition
- os
- pandas
- nltk
- matplotlib

Before doing Sentiment Analysis using NLTK, make sure to run the following command to get the pretrained corpus to work with : **nltk.download("all")**

Steps involved in Transcribing are:
- Extracted audio in WAV format from video
- Normalizing the audio
- Splitting audio into chunks based on Silence
- Using Google Speech Recognition API on the audio to get the transcript

Steps involved in sentiment analysis are:
- Preprocessing the text (tokenize, remove stopwords, lemmatize)
- Using SentimentIntensityAnalyzer get polarity scores for each sentence
- Based on a logic of scores, map the Sentiments to the Sentences
