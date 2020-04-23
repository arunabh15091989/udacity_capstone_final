# Data Scientist Nanodegree: Capstone Project

*The goal of this project is to detect the breed of a dog using Convolutional Neural Network (CNN). The pipeline implemented will detect if an image has a dog or a human and then make a prediction of the dog’s breed or the breed, which the human most resembles.*



[//]: # (Image References)

[image1]: ./static/img/ref/Anatolian_shepherd_dog.jpg "Sample Output"



## Project Overview

Welcome to the DogBreed Classifier project in the DS Nanodegree! In this project, you will learn how to build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, your algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  

![Sample Output][image1]

Along with exploring state-of-the-art CNN models for classification, you will make important design decisions about the user experience for your app.  Our goal is that by completing this lab, you understand the challenges involved in piecing together a series of models designed to perform various tasks in a data processing pipeline.  Each model has its strengths and weaknesses, and engineering a real-world application often involves solving many problems without a perfect answer.  Your imperfect solution will nonetheless create a fun user experience!


### Software Requirements
* Python 3.x
* Numpy
* Pandas
* Matplotlib
* Scikit-Learn
* Keras
* Tensorflow
* OpenCV
## Project Instructions

### File Description
1. dog_app.ipynb: Jupyter notebook explaining the process.

2. app.py: final flask app to run locally and predict dog breed or human.

3. dog_identification.py: uses utility functions of resnet50_dog.py and dog_classifer.py to predict dog breed.

### Data Preprocessing Steps used
1. Image is read.
2. Converted from RGB to Gray Scale.
3. Images are then converted to a matrix for training.

### Metric Used
Metric used is accuracy. The reason for choosing accuracy is because we need to find number of correct dog breed classifications out of total to tes model performance. Any other metric like AUC or Sensitivity, Precision etc. will not be as useful and simple to understand.

### Results obtained:
1. VGG16 - 42%
2. Inception - 78%
3. Model from scratch - 7%

### Instructions
1. Clone repo
	```
		git clone https://github.com/arunabh15091989/udacity_capstone_final.git

		cd udacity_capstone_final
	```
2. Download necessary requirements
	```
		pip install -r requirements.txt
	```
3. Run
	```
		python app.py
	```
4. Browse to http://localhost:5000
5. Upload Image files
