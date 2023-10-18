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


<!-- 
To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    --- -->
<!-- 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div> -->
<!-- <div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %} -->
