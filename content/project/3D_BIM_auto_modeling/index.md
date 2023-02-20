---
title: "Automated 3D BIM modeling for Digital Twin development"
subtitle: 3D point cloud object detection, using H3DNet object detector and REVIT APIs
layout: post
date: 2020-07-30 12:38:00 +0700

draft: false
featured: false

tags:
  - Python
  - 3D point cloud
  - Tensorflow
  - LiDAR
  - 3D object recognition
  - REVIT APIs
  - 3D BIM 
  - C#
  - Database
  - IoT
  - Simulation
  
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
This project focuses on **fully automatically 3D BIM modeling** using 3D point cloud data.
In this project, we firstly collected 3D point cloud data of small room by using **iPhone 12 Pro** (integrated LiDAR sensor). The collected data then will be treated as input data of 
3D point cloud recognition model. This deep learning model was trained on both public dataset (ScanNet V2) and our private dataset. \
For constructing 3D BIM model from predicted results, we developed an application based on REVIT APIs (C#) that can automatically construct 3D BIM model of room inside objects such as wall, 
floor, ceiling, tables, chairs, cabinets, etc. These 3D BIM models of the room can be integrated with our Digital Twin System or with IoT sensor database for simulation.



