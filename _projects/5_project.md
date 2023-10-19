---
layout: page
title: 5
description: Skin Cancer Lesion Classification
img: assets/img/pro5.png
importance: 5
category: work
---
Background: The principal objective of this project is to diagnose seven categories of skin diseases including Melanoma, Melanocytic nevus, Basal cell carcinoma, Actinic keratosis / Bowen’s disease, Benign keratosis, Dermatofibroma, and Vascular lesion.

Method: I used the HAM10000 dataset, which is a large collection of multi-source dermatoscopic images of common pigmented skin lesions. Firstly, I preprocessed the input data by normalizing and resizing the images. Furthermore, as the dataset was imbalanced, I implemented several methods to overcome the imbalanced data set problem. I augmented the data and tried oversampling as well as employing the XGBoost algorithm which is well-known for boosting imbalanced dataset performance. For the main classification, I used convolutional neural networks with different architectures 

Results: The final model could obtain 72.7% accuracy using CNN as the feature extractor and XGBoost as the classification head.
See more detailes and implementation in my <a href='https://github.com/afroozsheikh/HAM1000-Skin-Cancer'>Github</a>
