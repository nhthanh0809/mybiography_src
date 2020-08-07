---
title: ""

# View.
#   1 = List
#   2 = Compact
#   3 = Card
#   4 = Citation
view: 4

# Optional header image (relative to `static/img/` folder).
header:
  caption: ""
  image: ""
---


draft: false
featured: true
  
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
    url: 'https://github.com/smahesh2694/3D_detection_and_tracking_ROS/'
    
---

Vision sensor data (RGB and Depth) collected from a **semi-humanoid robot** ‘Pepper’ provided by IATSL laboratory, 
are used to perform 3D human detection and tracking within a household setup enabling better assistance to old or 
sick-adults in home-care. Implemented **YOLOv3** for 2D detection and used the **depth map** to cluster the 3D region of the 
patient, which is passed to an Extended Kalman Filter in ROS environment to track the patient.

Clone the workspace provided on Github and build it. 

Reproduce the results using launch command,
```
$ roslaunch det_and_tracking
```

{{% alert note %}}
If it throws an error, create a new workspace following ros tutorials 
and copy `/src`'s contents to the New workspace's  `src` and re-build it. 
{{% /alert %}}
