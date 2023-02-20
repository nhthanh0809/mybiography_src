---
title: "Synthesizing data by using 3D object models"
subtitle: Synthesizing panoramic images data for object recognition without real images
layout: post
date: 

draft: false
featured: true

tags:
  - Python
  - Pytorch
  - Tensorflow
  - Deep Learning
  - 3D
  - YoloV5
  - OpenCV
  - EfficientDet
  - Mask-RCNN
  
external_link: 

image:
  filename: featured.png
  focal_point: Smart
  preview_only: false
  caption: 
 
---
In this project, we focus on synthesizing 360 panoramic image data from 3D models without real image.
We first collected 3D models of in-house objects such as table, curtain, chairs, air-conditioner, TV, etc from [online storage](https://3dwarehouse.sketchup.com/).
We then rendered these 3D model on a license software for visualizing 3D models. 
We chose this software because it has a function that allowing rendering objects under virtual 360 degrees camera. Using this software, we generated virtual multi-view video and images of collected 3D objects.
Next, the videos and images will be processed by own developed tool allowing segment objects from background images.
This tool synthesized 360 panoramic image data by putting segmented object images on different background. \
Finally, we trained some well-known object detectors (YoloV3, YoloV5, EfficientDet, Mask-RCNN, etc.) on the synthesized data then evaluated on 360 degree public dataset namely [360-Indoor](https://openaccess.thecvf.com/content_WACV_2020/html/Chou_360-Indoor_Towards_Learning_Real-World_Objects_in_360deg_Indoor_Equirectangular_Images_WACV_2020_paper.html)
The evaluation results show that this method is very efficient, low-cost and promising approach for synthesizing 360 image dataset.
