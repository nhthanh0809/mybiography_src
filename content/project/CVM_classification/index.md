---
title: "Fully automated Cervical Vertebral Maturation assessment"
subtitle: Classifying Cervical Vertebral Maturation (CVM) by AI approach.
layout: post
date: 

draft: false
featured: false

tags:
  - Python
  - Pytorch
  - Medical image analysis
  - Cephalometric
  - Landmark detection
  - Deep learning
  - Machine Learning
  - Catboost
  - XGBoost
  - LightGBM
  - Bioimage informatics
  
external_link: 

image:
  filename: featured.png
  focal_point: Smart
  preview_only: false
  caption: 
links:
  - icon_pack: fab
    icon: github
    name: View Code 
    url: ''
---
Cervical vertebra maturation (CVM) staging in lateral cephalometric radiographs is an efficient method to determine skeletal maturation, 
as lateral cephalometric radiography is routinely required for orthodontic diagnosis and treatment planning in orthodontic practice with no additional radiographs required to assess the CVM stages. 
In this researching theme, we researched and developed an application applied AI algorithms that were trained on 
public dataset of Cephalometric image [ISBI 2015](https://biomedicalimaging.org/2015/program/isbi-challenges/) for classifying CVM stages. \
We firstly annotated CVM landmarks and CVM class label for 400 images in [ISBI 2015](https://biomedicalimaging.org/2015/program/isbi-challenges/).
The annotated data were reviewed by 4 doctors (2 junior and 2 senior) to ensure reliability.
Subsequently, the landmarks data first was trained with deep learning landmark detection model. The model achieved 99.42% [Success Detection Rate (SDR)](https://pubmed.ncbi.nlm.nih.gov/25794388/) with respect to the 2mm precision range. \
After getting output from landmark detection model, we calculated our proposed cervical stage score values (the Figure) following to this [User' Guide](https://pubmed.ncbi.nlm.nih.gov/29337631/).
These score values closely follow to CVM assessment features that were introduced by [Baccetti et al.](https://www.sciencedirect.com/science/article/abs/pii/S1073874605000216).
Finally, these calculated score values and annotated CVM class labels were treated as input tabular data for training different classification model such as Multi-Layer Perceptron (MLP), CatBoost, XGBoost, and LightGBM. 
These models will output 6 CVM stages from CS1 to CS6 as final results. \
NOTE: These tools currently has been integrated with other advanced technology tools in [Viceph](https://www.viceph.net/) - an online AI driven application for orthodontist.

