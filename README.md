# Multimodal Sentiment Analysis and Caption Generation

## Overview

This repository contains a versatile Python codebase for performing multimodal analysis, integrating both sentiment analysis and caption generation on a provided dataset. The code adopts a systematic approach to preprocess textual and image data, utilizing GloVe word embeddings for sentiment analysis and a ResNet-50 model for image feature extraction. Sentiment analysis is executed through a Multimodal Sentiment Analysis model that synergizes textual and image features.

## Features

Sentiment Analysis: Utilizes GloVe word embeddings and a ResNet-50 model to perform sentiment analysis.

### Caption Generation Extension:

Introduces an extension for caption generation on positive sentiment data, isolating and splitting it into training and testing sets. The MultiModalCaptionGeneration model, featuring an LSTM for text processing and a CNN for image processing, predicts the next word in the caption during training and generates captions during testing.

### Datasets and Dataloaders:

Custom datasets (CaptionDataset for training and CaptionTestDataset for testing) and dataloaders are tailored for both training and testing phases.

### Model Training and Evaluation:

Trains the model using the defined datasets and evaluates its performance on the test set. The model generates captions for each test image, and the results are written to a file named predicted_captions.txt.

## Usage

Ensure required dependencies are installed: gensim, torch, torchvision, numpy, pandas, sklearn, and PIL.

## Conclusion

This combined code exemplifies the flexibility and efficacy of a unified model designed to handle diverse tasks, seamlessly integrating sentiment analysis and caption generation in a multimodal context. Feel free to adapt and extend the code for your specific use cases.
