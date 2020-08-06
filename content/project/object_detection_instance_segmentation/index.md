---
title: "Object Detection and Instance Segmentation"
subtitle: Instance segmentation on stereo vision images of KITTI dataset, using YOLOv3 object detector and depth data.
layout: post
date: 2020-07-30 12:38:00 -0700

draft: false
featured: false

tags:
  - Python
  - YOLOv3
  - Segmentation
  
external_link: 

image:
  filename: featured.png
  focal_point: Smart
  preview_only: false
  caption: YOLO detections, calculated Depth and Segmentation mask
links:
  - icon_pack: fab
    icon: github
    name: View Code 
    url: 'https://github.com/smahesh2694/Object_Detection_and_Instance_Segmentation'
---
This assignment focuses on 2D object detection and instance segmentation using the
depth data. Motivated by the KITTI vision challenge for object detection and tracking, disparity
map between the corresponding images from left (p2) and right (p3) camera are provided. Depth
map for all images are estimated using the given disparity and calibration information, and the
results are attached along the submission as advised. An off-the-shelf configured 2D object
detection algorithm YOLO v3 pre-trained on COCO dataset is provided for direct implementation.
By tuning the confidence and non-maxima suppression threshold values, all cars in the frame of
left image are detected and attached in this report. For each detection of objects with label ‘car’,
the average depth is calculated neglecting the values with zero depth. Then a heuristic way for
instance segmentation is implemented, to calculate the range of depth values to be considered
as that of car, based on the average depth. More detailed information regarding the
implementation is provided under each corresponding section. 

**NOTE:** Please upgrade to the latest opencv version to avoid errors.

1. Kindly create new folders inorder to save results.
	<ul>
		<li>data/test/est_depth</li>
		<li>data/test/yolo</li>
		<li>data/test/est_segmentation</li>
	</ul> 
	
2. The bounding boxes are saved as numpy arrays and accessed later 
during the instance segmentation process. So it's important to follow step 1.
