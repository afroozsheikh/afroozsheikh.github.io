---
layout: page
title: 1
description: Autism Spectrum Disorder Diagnosis Using Graph Neural Network from brain fMRI data
img: assets/img/pro1.png
importance: 1
category: work
related_publications:
---

Background: Autism Spectrum Disorder (ASD) is a psychiatric disorder that leads to communication impairment. My main purpose in this project was to identify ASD patients from healthy controls given fMRI data from ABIDE1 dataset. ABIDE I involved 17 international sites, sharing previously collected resting state fMRI including 539 from individuals with ASD and 573 from typical controls.

Method: In this project, I focused on the automated detection of autism spectrum disorder using two distinct variants of  graph neural networks including Graph Attention Neural Network (GAT) and GraphSAGE. I utilized Nilearn library to fetch the ABIDE dataset and then I extracted fMRI time series from ROIs in the atlas.  Then, I constructed a graph using functional connectivity matrix obtained from calculating the correlation between the time series for each subject. Having built the graph, I took advantange of Graph Neural Networks for classifying each subject as ASD or healthy control. For the construction of graph neural networks, I used PyTorch and PyTorch Geometric packages. Furthermore, I applied two graph data augmentation (GDA) techniques to this problem and compared the results.


Challenges: In this project, I faced some challenges including working with the large brain imaging dataset (ABIDE) not only because of its huge size but also for my lack of knowledge and expertise in working with functional magnetic resonance imaging (fMRI) data. However, it was a highly pleasurable project as I acquired a satisfactory comprehension of GNNs and fMRI data. 

See more detailes and implementation in my <a href='https://github.com/afroozsheikh/ASD_Diagnosis_Abide'>Github</a>
