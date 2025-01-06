# Image Classification Model for Rose and Sunflower using Teachable Machine

## Table of Contents 
[1- Introduction](#1--introduction)

[2- Project Structure](#2--project-structure)

[3- Steps to Run the Code](#3--steps-to-run-the-code)

[4- Code Explanation](#4--code-explanation)

[5- Example Output](#5--example-output)

[6- Conclusion](#6--Conclusion)

---
## 1- Introduction
This project aims to build an image classification model using Google’s Teachable Machine, designed to classify images into two categories: “Rose” and “Sunflower” The model is trained using images of these categories and is used to predict the correct category for a new image.

## 2- Project Structure
-	model.savedmodel/: Directory containing the trained TensorFlow model.
-	labels.txt: A file containing the class labels (Rose, Sunflower).
-	predict_image.py: A Python script to load the model, process the input image, and make predictions.

## 3- Steps to Run the Code
**1. Install Required Libraries:**

     - To run the code, install the following libraries: 
       pip install tensorflow pillow numpy
     
**2. Prepare the Image:**

     - Place the image you want to classify in the same folder as the script, or provide the full path to the image.
**3. Run the Script:**

     - To run the script and make a prediction, use the following command: python VisionAI.ipynb
**4.	Review the Results:**

     - The model will output the predicted label (Rose or Sunflower) along with the confidence level of the prediction.

## 4- Code Explanation
- Loading the Model: The trained model is loaded using tf.saved_model.load from the model.savedmodel/ directory.
- Image Preprocessing: The image is resized to the required dimensions (224x224) and converted to a Tensor.
- Prediction: After preprocessing the image, it is passed through the model to get the prediction, and the class with the highest probability is selected.

## 5- Example Output
![Screenshot 2025-01-07 012944](https://github.com/user-attachments/assets/9f1b9acb-5123-4d26-9459-1f2967ba0053)

![Screenshot 2025-01-07 012621](https://github.com/user-attachments/assets/60b4d530-4962-474b-8599-2e8dba49e6c3)

## 6- Conclusion
This project uses Teachable Machine to create a simple yet accurate image classification model that distinguishes between two types of images: “Rose” and “Sunflower,” allowing the correct category to be predicted for any new image.
