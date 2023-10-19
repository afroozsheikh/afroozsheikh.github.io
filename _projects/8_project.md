---
layout: page
title: 8
description: Date translator
img:
importance: 8
category: work
---

Goal: Translate any format of date input to its corresponding “yyyy-mm-dd” format

Tools and frameworks: Recurrent neural network (RNN) architecture using Bidirectional Long short-term memory cell (Bi-LSTM), both Attention layers were implemented using Keras.

Approach and architecture:  First, we preprocess the input string to convert all of its characters to the corresponding indexes, then the result was passed to the Bi-LSTM layer to get the string state, then passed to an attention layer followed by an LSTM layer, and finally pass every LSTM cell output to a SoftMax function to predict the index of the output string.

Outcome: The final package was able to take a maximum of 36-characters sentences and predict the “yyyy-mm-dd” format of the input string.