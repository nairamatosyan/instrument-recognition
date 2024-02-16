# instrument-recognition

## Introduction
The goal of the project is to create a deep learning model that can recognize musical instruments from audio samples.

## Feature Extraction
The Mel Spectogram is extracted from audio samples using the Librosa library. The Mel Spectrogram is a visual representation of the spectrum of frequencies of a signal as they vary with time. The Mel Spectrogram is a 2D array of shape (n_mels, t) where n_mels is the number of mel bands and t is the number of frames.

## Classification
The models are trained using the Adam optimizer and the categorical cross-entropy loss function. The dataset is divided into training and testing setsand they are trained on the training set and evaluated on the testing set using the confusion matrix and accuracy metric. The models are also evaluated on a separate dataset of audio samples of different musical instruments.
Two models are trained: a Convolutional Neural Network (CNN) and a Long Short-Term Memory (LSTM) network.

## Dataset
The dataset used is the IRMAS dataset. The dataset contains 6705 audio samples of 11 different musical instruments. The dataset is divided into 11 different folders, each folder contains audio samples of a different musical instrument. The dataset is available at: https://www.upf.edu/web/mtg/irmas