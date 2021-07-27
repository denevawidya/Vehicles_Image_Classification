# Image Classification Model Deployment of Vehicles and Non-Vehicles

- Dataset : [Kaggle - Vehicle-Detection](https://www.kaggle.com/brsdincer/vehicle-detection-image-set)

In this project I'm trying to develop an ML model for image classification and then convert the model into a TF-Lite file format that can be embedded in Android and iOS. Here I'm also still using TensorFlow that will help identify the vehicles or non vehicles images

## Modelling

All the steps are more or less the same as the [RPS Image Classification](https://github.com/denevawidya/RPS_Image_Classification).

The steps taken include:
1. Download the dataset and extract the file with the unzip method.
2. Store the directory of each class in the train directory and validate it into a variable.
3. Use Image Data Generator Tensorflow for image processing and split the datasets into train and validation (20%)
4. Prepare training data that will be studied by the model.
5. Modelling with Sequential and using Conv2D Maxpooling Layer.
6. Compile and train the model with model.compile and model.fit until you get the desired accuracy.
7. Predict the images of Vehicles or Non-Vehicles.
8. Save the model into TF-Lite format.

## Results

The model has an accuracy of up to 98% and can predict the images of Vehicles

![image](https://user-images.githubusercontent.com/87906938/127177073-61c7c159-108b-4dee-ab80-48b60d41a2e2.png)

![image](https://user-images.githubusercontent.com/87906938/127176880-a2b5832a-5cfc-47f6-87fe-b5f4d587e057.png)

Also successfully export the model into TF-Lite

![image](https://user-images.githubusercontent.com/87906938/127177002-1555ea1a-1f25-4a1b-a242-e524dfd5abbd.png)

