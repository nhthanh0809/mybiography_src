---
title: "Automatic Cephalometric landmark detection"
subtitle: Landmark identification with deep learning approach on ISBI dataset.
layout: post
date: 

draft: false
featured: false

tags:
  - Python
  - Pytorch
  - Tensorflow
  - Medical image analysis
  - Cephalometric
  - Landmark detection
  - Deep learning
  - Biomedical imaging

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
**Landmark identification** is crucial in quantifying cephalometric analysis such as Steiner, Bjork, Ricketts, Kim, Nagasaki, etc. For applying these analysis to cephalometric image, dentist or orthodontist need to annotate 
some group of landmarks that corresponding to specified analysis. Manual annotation of landmarks is a tedious, laborious task and prone to human errors. 
Therefore, it's necessary that they need an efficient automated application for landmark identification. \
In this project, we developed an online efficient AI driven tools for automatically detecting landmark on Cephalometry image. 
The core part of these tools is our developed deep learning model with backbone ***DenseNet121***. This model was trained on both public dataset of Cephalometric image [ISBI 2015](https://biomedicalimaging.org/2015/program/isbi-challenges/) and private dataset. \
These tools currently has been integrated with other advanced technology tools in [Viceph](https://www.viceph.net/) - an online AI driven application for orthodontist.

