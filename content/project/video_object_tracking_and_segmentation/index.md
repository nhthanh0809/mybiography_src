---
title: "Video object tracking and segmentation for digital camera"
subtitle: Optimizing object tracking and segmentation model for running on digital camera 
layout: post
date: 

draft: false
featured: true

tags:
  - Python
  - Pytorch
  - Tensorflow
  - Deep Learning
  - Objet Segmentation
  - Object Tracking
  - C++
  - MobileNet
  - Quantization
  - Pruning
  - Camera
  
external_link: 

image:
  filename: featured.png
  focal_point: Smart
  preview_only: false
  caption: 
 
---
In this project, we focus on optimizing **video object tracking and segmentation** model for running on digital still camera.
We used the Siamese network based model for tracking object on input video. The model was trained on larger video dataset such as Youtube-VOS, ImageNet-VID 2015, etc. \
For optimizing the model, firstly we change backbone of the model from ResNet50 to MobileNetV1. We then re-trained and re-evaluated the modified model on above datasets.
The evaluation show that while accuracy of the new model slightly decrease but performance significantly increase in comparison with the original one. \
Next step, we implemented quantization and pruning methods for compressing the model weight from Float 16 to Int 8, in order to it can run on edge device like digital camera.


