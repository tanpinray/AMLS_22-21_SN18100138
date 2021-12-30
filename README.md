# ELEC0134 Applied Machine Learning Systems Coursework 2021

## Introduction
The need for accurate automated brain tumor classification from medical images is crucial to improve medical analysis and diagnosis. This field has been studied for decades and several methods have been proposed. In this project, two brain tumor identification tasks will be attempted with ML classification techniques: Task A which is to identify the presence of a brain tumor in a MRI image; and Task B which is to identify the type of brain tumor in a MRI image. Two models are implemented for the tasks: One which extracts textural features from images using Histogram of Orientated Gradients (HOG), Local Binary Pattern (LBP) and Discrete Wavelet Transform (DWT)  methods, followed by using popular classifiers Support Vector Machines (SVM) and K-Nearest Neighbours (KNN); and another Convolutional Neural Network (CNN) based model which utilizes tranfer learning from a pre-trained Xception architecture to extract features and classify images. It was observed that using HOG and DWT features with RBF kernel SVM performed well in both tasks, with an accuracy of 98% and 95% respectively, whereas the CNN slightly underperformed in identifying brain tumor types, achieving and accuracy of 91%.

Three main 

## Instructions
The instructions to 
The training dataset can be downloaded from this URL: http://shorturl.at/hquDP

The test dataset can be downloaded from this URL: https://drive.google.com/file/d/1LS_C_4_iOeqOyEoWPPoksrk8lqdBKagB/view
