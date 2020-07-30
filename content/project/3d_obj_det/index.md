---
title: "3D Object Detection and Tracking"
subtitle: Course project
layout: post
date: 2020-07-30 12:38:00 -0700

draft: false
featured: false

tags:
  - Makefile
  - CMake
  - C++
  - Python
  - YOLOv3
  - EKF
  
external_link: 

image:
  filename: featured.png
  focal_point: Smart
  preview_only: false
  caption: defect highlight  
 
---

Vision sensor data (RGB and Depth) collected from a **semi-humanoid robot** ‘Pepper’ provided by IATSL laboratory, 
are used to perform 3D human detection and tracking within a household setup enabling better assistance to old or 
sick-adults in home-care. Implemented **YOLOv3** for 2D detection and used the **depth map** to cluster the 3D region of the 
patient, which is passed to an Extended Kalman Filter in ROS environment to track the patient.
