---
layout: page
title: 4
description: Nuclear Segmentation of Histology Images
img: assets/img/pro4.jpg
importance: 4
category: work
---
Background: Nuclei segmentation in histology images has received much attention in the past few years as a requirement for cell detection, cell classification, and cancer grading. My ultimate goal in this project was to segment these nuclei as well as classify them to eight labels:  normal epithelial, malignant/dysplastic epithelial, fibroblast,
muscle, inflammatory, endothelial or miscellaneous.

Method: CoNSeP (Colorectal Nuclear Segmentation and Phenotypes) dataset is utilized in this project. The dataset consists of 41 image, each of size 1000×1000 pixels.  I took advantage of the segmentation models package for implementation of the U-net model, an encoder-decoder network for the segmentation task.  Finally, the model is able to predict the label for each pixel in the test data.

Results: The model is evaluated using two metrics of Intersection over union (IoU) and Dice score.

See more detailes and implementation in my <a href='https://colab.research.google.com/drive/1OQY5y_umKXU3A8uBIJ1eiqEiw8jG8118?usp=sharing'>Colab</a>
