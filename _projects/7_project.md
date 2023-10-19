---
layout: page
title: 7
description: Trigger word detection
img:
importance: 7
category: work
---
Goal: recognize trigger words (a.k.a “activate”) given short audio data.

Tools and frameworks: 1D Convolutional neural network, Recurrent neural network (RNN) architecture made up of Keras-implemented Gated Recurrent Units (GRU).

Approach and architecture: Conventionally, the dataset for the trigger word detection task is created manually for two reasons: first, it takes a lot of time to record audio clips with both trigger words and other commands, and second, it can be difficult to precisely label a recorded audio clip. Instead, we can merge a random 10-second background sound, 0–4 random trigger words, and 0–2 other commands to create each training and test sample. As a result, we are able to provide precise labels for each sample because we are aware of the precise moment the trigger phrase is introduced into the audio. We compute a spectrogram of the raw audio and then generate our dataset as was explained earlier to make it easier for your sequence model to learn to recognize trigger words. After extracting low-level data features from the spectrograms using a 1D Conv layer, the data is then sent to a two-layer recurrent neural network in which 128 Gated Recurrent Units (GRU) are used in each layer to evaluate the context of the input spectrograms. In order to determine whether the trigger word is being pronounced at this time stamp, we transmit each GRU output to a softmax layer. Finally, our mode predicts 1 if the trigger word is being said at the time stamp, and 0 otherwise.
