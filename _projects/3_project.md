---
layout: page
title: 3
description: Drug-drug Interaction Prediction
img: assets/img/pro3.png
redirect: 
importance: 3
category: work
---
Background: Due to the popularity of using multiple drugs for the treatment of complex diseases, drug-drug interactions (DDI) may give rise to the risk of unanticipated adverse effects and even unknown toxicity. In this project, I aimed to predict drug-drug interactions given information on already known drug-drug interactions. Each node represents an experimental drug and edges represent interactions between drugs.

Method: I used the obgl-ddi dataset to predict interactions between drugs. The task was link prediction and I used two approaches for this prediction. Firstly, I used the Node2vec algorithm for learning the embeddings of the given graph. Node2vec randomly walks and tries to make a balance between local and global structures of the graph. Then the result of dot production of 2 node embeddings(both positive and negative edges) will pass through some linear layers to make a prediction. My second approach was to utilize a graph neural network which consisted of three GCN layers and three linear layers following them.

Results: The evaluation metric for this project is Hits@K. The hits@k describes the fraction of true entities that appear in the first k entities of the sorted rank list

See more detailes and implementation in my <a href='https://github.com/afroozsheikh/Drug-Drug-Interactions'>Github</a>
