# Densely Populated Regions Face Masks Localization and Classification Using Deep Learning Models

<p align="center">
  <b>Anh Pham H.N., Linh Phung K., Vi Le T.T. and Nga Ly T.</b></span>
</p>

## Introduction
Welcome to the official codebase for the research "Densely Populated Regions Face Masks Localization and Classification Using Deep Learning Models" by our team from [International University - VNU-HCM](https://hcmiu.edu.vn/en/) with:
- @barbatoz0220 - Anh Pham H.N. as 1<sup>st</sup> author
- @indigoYoshimaru - Linh Phung K. as 2<sup>nd</sup> author
- @lttvi - Vi Le T.T. as 3<sup>rd</sup> author
- and [Dr. Nga Ly T.](https://it.hcmiu.edu.vn/user/ltnga/) as supervisor

## Overview
Over the last two years, the correct wearing of facial masks in public is still a relevant matter in the fight against the COVID-19 pandemic.
A popular approach that helps regulate this by global researchers is the application of Deep Learning.
This paper will contribute to the literature in two main aspects:

1. We first compare and contrast the application of four pre-trained models in classification of the specific face mask dataset.
2. We follow with the proposal of a face mask detector model which combines the state-of-the-art RetinaFace to the localization of faces in densely populated regions and the most prominent classifier obtained from the previous step to divide the faces into three categories: correctly-worn, incorrectly-worn and no-masks-worn.

## Results
Performance metrics from the test phase have shown that our detector were one to achieve the best accuracy among all works compared with 94,59% on one test dataset and a less satisfactory 69.6% on another due to certain characteristics of the set. A worth-noting feature is how it can perform rather well in densely populated detection of masks wearing following the validity of how the masks are worn: correctly, incorrectly and without. Although there are still certain limitations to some of the class variance, the performance metrics have proved our effectiveness with the combination of ResNet50V1 and RetinaFace. It is certainly possible for our model in the future to be better optimized, evaluated and ultimately deployed into public usage through real-world applications.

A few images showing the model's ability to detect and classify in crowded areas:
- ![Densely_populated1](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/figures/maksssksksss110.png)
- ![Densely_populated2](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/figures/maksssksksss296.png)
- ![Densely_populated3](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/figures/maksssksksss52.png)

Faces classified as Incorrectly-worn by the proposed model:
- ![incorrect1](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/figures/test_00000066.jpg)
- ![incorrect2](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/figures/test_00000078.jpg)
- ![incorrect3](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/figures/test_00000745.jpg)
- ![incorrect4](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/figures/test_00001137.jpg)

More results are available at: 
- For Kaggle dataset: https://drive.google.com/drive/folders/1-NcuMfzLFJMzlM4S_eOjHYdpm38dXVGS?usp=sharing
- For MAFA dataset: https://drive.google.com/drive/folders/183coq12n0vbm0wO4P3r8ECkSouyueWcd?usp=sharing
## Contents
In this repository, you will be able to find:
1. A comparison between 4 backbone models for the classification stage (MobileNetV1, MobileNetV2, ResNet50V1, ResNet50V2)
using the Kaggle12K dataset in the folder [exported_model](https://github.com/barbatoz0220/FMD-RICE2021/tree/master/exported_models/trained-on-kaggle12k)
Results on the accuracy and loss of each are expressed through the following figures:
- ![MobileNetV1 and MobileNetV2](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/figures/mobilenets_acc_loss.PNG)
- ![ResNetV1 and ResNetV2](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/figures/resnet_acc_loss.PNG)
2. A comparison between our proposed model (with ResNet50V2 implemented) and another two (AIZOO and Neuralet) in the file [model_comparison.ipynb](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/model_comparison.ipynb). The following figure illustrates each model's performance on the two test sets. ![model_comparison](https://github.com/barbatoz0220/FMD-RICE2021/blob/master/figures/proposed-aizoo-neuralet.PNG)
3. The Google Colab file for our proposed model is available at: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/indigoYoshimaru/11a0f157ee6813c174b5e2b0eb4a36e0/mask_detector.ipynb)

### More documentation and updates will be coming soon
