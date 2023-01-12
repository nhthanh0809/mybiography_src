---
title: "Room layout recognition"
subtitle: 
layout: post
date: 

draft: false
featured: true

tags:
  - Python
  - Pytorch
  - Tensorflow
  - Deep Learning
  - Instance Segmentation
  - Torchserve
  - Docker
  - Kubenetes
  - Cloud
  
external_link: 

image:
  filename: featured.png
  focal_point: Smart
  preview_only: false
  caption: 
 
---
In this project, we focus on building-up an **Instance segmentation** model for recognizing drawing room layout data.
We trained and tested our model (Unet architecture) on both public dataset (Cubicasa, R3D) and own dataset (more than 1000 images of drawing layout) 
To ensuring generalization of the trained model, we added CVF-FP dataset (public) to test set for evaluation. \
After AI model development, we deployed the model on Torchserve - a Pytorch model serving framework, and integrated to Kubenetes system. The AI model
will be used for classifying room type, providing essential information for construction site works.



