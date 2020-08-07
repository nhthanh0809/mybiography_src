---
title: "IDC type Breast Cancer Classification"
subtitle: Course project of ECE1512 - Digital Image Processing
layout: post
date: 2020-07-30 12:38:00 -0700

draft: false
featured: true

tags:
  - Keras
  - TensorFlow
  - Python
  - Jupyter Notebook
  - Deep Learning
  
external_link: 

image:
  filename: featured.png
  focal_point: Smart
  preview_only: false
  caption: H&E stained pathology tissue
  
links:
  - icon_pack: fab
    icon: github
    name: View Code 
    url: 'https://github.com/smahesh2694/Breast_Cancer_Classification'
 
---

# Breast_Cancer_Classification

**Breast cancer classification on Keras** (based on the implementaion of CancerNet algorithm by Adrian Rosebrock [1]).

Breast cancer is the most common form of cancer in women, and invasive ductal carcinoma (IDC) is the most common form of breast cancer. Accurately identifying and categorizing breast cancer subtypes is an important clinical task, and automated methods can be used to save time and reduce error.

The goal of this script is to identify IDC when it is present in otherwise unlabeled histopathology images.
The dataset consists of 277,524 50x50 pixel RGB digital image patches that were derived from 162 H&E-stained breast histopathology samples.
These images are small patches that were extracted from digital images of breast tissue samples. 

The breast tissue contains many cells but only some of them are cancerous. 
Patches that are labeled "1" contain cells that are characteristic of invasive ductal carcinoma. 

The dataset was originally curated by Janowczyk and Madabhushi and Roa et al. but is available in public domain on Kaggle’s website. 

For more information about the data used, 
see [here](https://www.ncbi.nlm.nih.gov/pubmed/27563488) and [here](http://spie.org/Publications/Proceedings/Paper/10.1117/12.2043872).

Reference:
[1]. Adrian Rosebrock, Breast cancer classification with Keras and Deep Learning, PyImageSearch, https://www.pyimagesearch.com/2019/02/18/breast-cancer-classification-with-keras-and-deep-learning/ , accessed on 22 February 2019.

