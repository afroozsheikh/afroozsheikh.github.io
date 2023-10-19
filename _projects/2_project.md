---
layout: page
title: 2
description: Detection of Specific Language Impairment
img: assets/img/pro2.jpg
importance: 2
category: work
# giscus_comments: true
---
Background: specific language impairment (SLI), is a language disorder that delays language development in children who have no hearing problems, neurological dysfunctions, or other developmental delays. Detecting SLI at an early stage is very important for successful speech therapy in children. Detecting whether an utterance is healthy or SLI from the only existing speech dataset for SLI from the LANNA laboratory was our main objective in this project.

Method: Firstly, I extracted some features from the audio clips using the open-smile library. Then the preprocessed data was passed through several classifiers such as neural network, decision trees, SVM, AdaBoost, Xgboost, and stacking classifiers using the sklearn library. Next, we tuned our hyperparameters for achieving the best results. After hyperparameter tuning and evaluation, we extracted more features using another feature set in the open-smile library which resulted in higher accuracy.  

See more detailes and implementation in my <a href='https://github.com/afroozsheikh/Detection-of-Specific-Language-Impairment'>Github</a>

