# Drone-Gesture-Recognition 🏆🏆🏆
A robust system for controlling drones using real-time hand gesture recognition. This project leverages computer vision and machine learning techniques to detect and interpret human gestures, enabling intuitive and contactless control of drones.

## Dataset_fn.ipynb 🚀
Creates a dataset for hand gestures corresponding to all the different movements a drone can make therefore
1.Left
2.Right
3.Forward
4.Up
5.Down
6.Flip
7.Rotate(by 90 degrees)

This uses **Mediapipe** Hand detection and Landmark model to create a dataset this uses **openCV** to capture different Landmark coordinates for your hand and compile those into a dataframe.
![image](https://github.com/user-attachments/assets/1e7f1188-051f-4eaf-8da6-5a8b52ca79ad)

Our dataframe looks like this at the end
![image](https://github.com/user-attachments/assets/6ae7d376-c0d1-46d4-92ff-b62cf5e98be1)

Now this data is taken for different gestures.This is then ready to train and test on our Neural Network.

## Create_model.ipynb🧑🏻‍💻
This file is used to create a model using artificial neural network that gives us an accuracy of **98.48%**.
Our dataset is splitted into train and test datasets and then model is trained over this data.

**64->128->64->32->16->8** 8 outputs for 8 different classes/gestures of the output 

Later on, this model is saved into a .h5 file that is used to hold large datasets or models.


