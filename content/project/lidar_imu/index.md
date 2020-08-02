---
title: "Lidar and IMU calibration"
subtitle: Course project of AER 1514 - Mobile Robotics
layout: post
date: 2020-07-30 12:38:00 -0700

draft: false
featured: false

tags:
  - ROS
  - Python
  - Matlab
  - Linux
  
external_link: 

image:
  filename: featured.png
  focal_point: Smart
  preview_only: false
  caption:  
 
---

Worked on a 6 DOF non-linear optimization problem to determine the pose vector relating an Inertial Measurement 
Unit (IMU) to a LiDAR sensor based on the data collected on **Zeus self-driving car** during its operation.


<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" width="161px" viewBox="-0.5 -0.5 161 161" content="&lt;mxfile host=&quot;app.diagrams.net&quot; modified=&quot;2020-08-02T18:51:20.536Z&quot; agent=&quot;5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.89 Safari/537.36&quot; etag=&quot;kmGgtXMmF9i3SAWSXesK&quot; version=&quot;13.5.4&quot; type=&quot;github&quot;&gt;&lt;diagram id=&quot;IBLU77m72bvmYz1W5Is1&quot; name=&quot;Page-1&quot;&gt;jZNNU4MwEIZ/DUdn+BhrexSserDjAcfaY5psIWNgMU0L9de7yALFTmc8kX32M28WL0qK5smKKl+hAuOFvmq86MELw8CP5vRpyakjt3MGmdWKg0aQ6m/oM5ketIL9JNAhGqerKZRYliDdhAlrsZ6G7dBMu1YigwuQSmEu6VorlzMNZovR8Qw6y7n1PLzrHIXog/km+1worM9QtPSixCK67lQ0CZhWvF6XLu/xincYzELp/pOweVvj+2rz8vr1kSWRlNLfbm/CrspRmANfeJXyuO7Ua+CgoQ5x7gpDIKDj3ln8hAQNWiIllhQZ77Qxf5AwOivJlDQjEI+PYJ0mde/ZUWil2jZxnWsHaSVk27OmXSJm8VAqaMf3yeJJqQA0VyUIBmFpIwELcPZEIZxw228VL2O4YLs+e9oZs/zsVQcoeJ2yofaoOB1Y9N4cH/fXd/aLRMsf&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://viewer.diagrams.net/?client=1&amp;edit=_blank');}}})(this);" style="cursor:pointer;max-width:100%;max-height:161px;"><defs/><g><rect x="0" y="0" width="160" height="160" fill="none" stroke="none" pointer-events="all"/><g transform="translate(-0.5 -0.5)"><switch><foreignObject style="overflow: visible; text-align: left;" pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 158px; height: 1px; padding-top: 80px; margin-left: 1px;"><div style="box-sizing: border-box; font-size: 0; text-align: center; "><div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: #000000; line-height: 1.2; pointer-events: all; white-space: normal; word-wrap: normal; ">MS</div></div></div></foreignObject><text x="80" y="84" fill="#000000" font-family="Helvetica" font-size="12px" text-anchor="middle">MS</text></switch></g></g><switch><g requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"/><a transform="translate(0,-5)" xlink:href="https://desk.draw.io/support/solutions/articles/16000042487" target="_blank"><text text-anchor="middle" font-size="10px" x="50%" y="100%">Viewer does not support full SVG 1.1</text></a></switch></svg>
