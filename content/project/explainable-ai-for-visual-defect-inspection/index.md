---
title: Explainable AI for Visual Defect Inspection
subtitle: Graduate Dissertation
layout: post
date: 2020-07-24T18:07:40.013Z

draft: false
featured: true

tags:
  - XAI
  - Deep Learning
  - Python
  - Keras
  - TensorFlow
  - PyTorch
  - Git 
  - Research
  
external_link: 

image:
  placement: 3
  filename: featured.png
  focal_point: Smart
  preview_only: false
  caption: defect highlight
  alt_text: Defect highlight
  
links:
  - icon_pack: fab
    icon: github
    name: View Source Code 
    url: 'https://github.com/smahesh2694/NEU_XAI/'
    
  - icon_pack: fab
    icon: github
    name: Supplementary Code 
    url: 'https://github.com/smahesh2694/MVTec_GradCAM/'
    
---

Developed and studied XAI algorithms that generates saliency maps according to the importance of each corresponding pixels of the input test image towards the Machine Learning model's predictive accuracy, with the aim of decoding complex 'black-box' models. 

### [NEU_XAI](https://github.com/smahesh2694/NEU_XAI/)

This repo contains keras implementation of few XAI algorithms on [NEU surface defect dataset.](http://faculty.neu.edu.cn/yunhyan/NEU_surface_defect_database.html)

Repo consists of :
<ol>
  <li>NEU steel surface defect database --> Original 1800 image NEU dataset</li>
  <li>NEU steel surface defect database - Test Split --> contains 180 test images (with 10% partition)</li>
  <li>Finetune_on_NEU_dataset.ipynb --> 
    i) Training a MobileNet model on the NEU surface defect dataset using Transfer Learning.
    ii) visualizing the important features of test images using model agnostic LIME and SHAP algorithms.</li>
</ol>

Sample images from NEU dataset :
![Sample images from NEU dataset](https://github.com/smahesh2694/NEU_XAI/blob/master/NEU_dataset%20image.jpeg?raw=true)
