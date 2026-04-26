Skin Cancer Classification using NBI Images
Overview
This project focuses on the classification of skin cancer lesions using deep learning techniques. The goal is to build a model capable of identifying different types of skin lesions from medical images.
The project explores the use of EfficientNetB1, a convolutional neural network architecture, to classify skin lesion images into three categories.
An important aspect of this project is the use of Narrow Band Imaging (NBI) representation of skin lesion images to enhance visual features before training the model.

Problem Statement
Skin cancer is one of the most common forms of cancer worldwide. Early detection plays a crucial role in improving treatment outcomes. Medical image analysis using deep learning can assist dermatologists by providing automated classification of skin lesions.
This project investigates the use of deep learning models to classify skin lesion images into different cancer categories using medical image data.

Dataset of Skin Cancer:
Dataset consist of 3 Classes-
- BCC: Basal Cell Carcinoma
- SK: Seborrheic Keratosis
- Ak: Actinic Keratosis
Image format:
- Originally image were in RGB format or they were white light image.
- As described in the project methodology, converted the datset into Narrow Band Imaging(NBI) format before model training to enhance the feature extraction.
Dataset Split:
- Dataset was then splitted into 3 sunsets fro training and evaluation. 
- Train , Validation, and Test with the split ratio of 70:20:10.
Data Preprocessing:
- Before training the deep learning model, images were resized to match model input requirement. 
- Normalization of pixel values.
- Images were augumented using Data augumentation techniques like Rotation and flips. No contrast and color change of images were done to keep originality of image.
The dataset is not included in this repository due to size limitations and dataset usage restrictions.





