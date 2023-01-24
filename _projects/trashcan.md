---
layout: page
title: Intelligent garbage can
description: Design of Intelligent garbage can and Construction of sorting and Recycling system
img: assets/img/trashcan/trashcan.png
importance: 1
category: competition
link: true
new_page: true
---
Our team plans to launch a set of intelligent garbage classification regionalization control and management system to realize the regional management of garbage cans. Transform the traditional garbage bins in urban streets, communities, campuses and other public places to realize the functions of induction switch, intelligent classification, internal space adjustment, automatic packaging and anti-overflow, and adopt Lora technology to realize the regional control and management of garbage bins, which can improve the efficiency of garbage recovery and the degree of resource utilization.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/trashcan/trashcan2.png" title="Work flow chart of intelligent system" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Work flow chart of intelligent system.
</div>

Our products are composed of the following three parts:
<br>
<b>First, intelligent sorting of trash bins.</b>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/trashcan/trashcan.png" title="Work flow chart of intelligent system" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<br>
The intelligent sorting trash can has the functions of automatic classification, automatic packaging, wireless network connection, real-time online monitoring in the background, real-time data transmission of trash can capacity and so on.
<br>
By crawling different types of spam image data and selecting a large number of available images from each category, we build a multi-layer convolutional neural network using Python and train the dataset, obtain a weight file, and test the trained model. The final requirement is to achieve a recognition rate of 95% or more.
<br>
OpenMV is an open source, low cost, powerful machine vision module. With STM32F427 CPU as the core and OV7725 camera chip integrated, the core machine vision algorithm is efficiently implemented in C language on a small hardware module, providing a Python programming interface.

<div class="row">
    <div class="col-sm mt-3 mt-md-0 pic_center">
        {% include figure.html path="assets/img/trashcan/trashcan5.png" title="Crawled data" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0 pic_center">
        {% include figure.html path="assets/img/trashcan/trashcan6.png" title="Crawled data" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<b>Second, the backstage monitoring center.</b>
<br>
<div class="row">
    <div class="col-sm mt-3 mt-md-0 ">
        {% include figure.html path="assets/img/trashcan/trashcan3.png" title="the backstage monitoring center" class="img-fluid rounded z-depth-1 " %}
    </div>
</div>
The background monitoring center realizes the data analysis and storage of the whole system, so that the staff can grasp the situation of each trash can at any time, and realize the real-time supervision and deployment of the designated garbage cleaning vehicles.

<b>Third, mobile phone terminal.</b>
<br>

The mobile phone terminal serves the city cleaners and garbage can managers, so that the staff can arrange the cleaning time reasonably. Greatly improve work efficiency.