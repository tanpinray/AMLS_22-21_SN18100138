# ELEC0134 Applied Machine Learning Systems Coursework 2021

## Introduction
The need for accurate automated brain tumor classification from medical images is crucial to improve medical analysis and diagnosis. This field has been studied for decades and several methods have been proposed. In this project, two brain tumor identification tasks will be attempted with ML classification techniques: Task A which is to identify the presence of a brain tumor in a MRI image; and Task B which is to identify the type of brain tumor in a MRI image. Two models are implemented for the tasks: One which extracts textural features from images using Histogram of Orientated Gradients (HOG), Local Binary Pattern (LBP) and Discrete Wavelet Transform (DWT)  methods, followed by using popular classifiers Support Vector Machines (SVM) and K-Nearest Neighbours (KNN); and another Convolutional Neural Network (CNN) based model which utilizes tranfer learning from a pre-trained Xception architecture to extract features and classify images. It was observed that using HOG and DWT features with RBF kernel SVM performed well in both tasks, with an accuracy of 98% and 95% respectively, whereas the CNN slightly underperformed in identifying brain tumor types, achieving and accuracy of 91%.

Three Jupyter Notebook files are in this project: Task_A, Task_B and Task_B_NN. The first two notebooks use SVM and KNN classifiers for the respective tasks, and the third notebook uses tranfer leaning.

## Instructions
The instructions to run the code is as follows:
1. Clone this repository to your local device
2. Download the training dataset from this URL: http://shorturl.at/hquDP
3. Extract the dataset directory from the zipped file downloaded in step 2, which contains the image folder with the MRI images and label.csv, which stores the class information for each image.
4. Download the test dataset from this URL: https://drive.google.com/file/d/1LS_C_4_iOeqOyEoWPPoksrk8lqdBKagB/view
5. Extract the test directory from the zipped file downloaded in step 4, which contains the image folder with the MRI images and label.csv, which stores the class information for each image.
6. From your computer's command prompt, move to the directory where the local repository is stored. For example, this can be done through entering the following command: cd {documents/github}/elec0134-amls-cw. The value in {} should be changed to reflect where the local repository is stored in your computer.
7. (Optional but Recommended) Create and activate a new virtual environment to install the necessary packages to run these files.
8. Install the required packages by entering the command pip install -r requirements.txt. If using Anaconda or Miniconda command prompt, steps 7 and 8 can be summarized into the following command: conda create -n amls-cw --file requirements.txt -c conda-forge

### Necessary packages
The necessary packages are as follows:
- python>=3.7.11
- numpy==1.21.4
- scipy==1.7.3
- matplotlib==3.5.0
- pandas==1.3.4
- tqdm==4.62.3
- ipywidgets==7.6.5
- scikit-learn==1.0.1
- scikit-image==0.18.3
- imgaug==0.4.0
- pywavelets==1.2.0
- tensorflow>=2.5.1
- notebook==6.4.1

### Task A
1. Activate the environment that the packages were installed in
2. Open Jupyter Notebook by typing jupyter notebook in the command prompt
3. Navigate to the repository and open the Task_A file
4. In the first code block in Section 2.3, change 'augmentation' to True or False to select whether the augmented images should be used in training and testing the classifier
5. In the first code block in Section 4.1, change the value of 'feature' to select which extracted features should be used in training and testing the classifier. The list of features that can be selected are 'hog', 'lbp','multidwt', 'hoglbp', 'hogdwt', 'lbpdwt', 'all'
6. Run all cells and wait for the classifier to finish training and observe its performance on the test images

### Task B
1. Activate the environment that the packages were installed in
2. Open Jupyter Notebook by typing jupyter notebook in the command prompt
3. Navigate to the repository and open the Task_B file
4. In the first code block in Section 2.3, change 'augmentation' to True or False to select whether the augmented images should be used in training and testing the classifier
5. In the first code block in Section 4.1, change the value of 'feature' to select which extracted features should be used in training and testing the classifier. The list of features that can be selected are 'hog', 'lbp','multidwt', 'hoglbp', 'hogdwt', 'lbpdwt', 'all'
6. Run all cells and wait for the classifier to finish training and observe its performance on the test images

### Task B (CNN-based Model)
1. Activate the environment that the packages were installed in
2. Open Jupyter Notebook by typing jupyter notebook in the command prompt
3. Navigate to the repository and open the Task_B_NN file
4. In the first code block in Section 2.4, change 'augmentation' to True or False to select whether the augmented images should be used in training and testing the model
5. Run all cells and wait for the classifier to finish training and observe its performance on the test images
