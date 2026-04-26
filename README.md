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

Model:

EfficientNetB1
Training approach:
- The model uses EfficientNetB1 as the backbone convonutional neural network.
- EfficientNetB1 was loaded with pretrained ImageNet weights.
- Added custom classification layers:
  - GlobalAveragePooling2d
  - Dense layer (128 units, ReLU)
  - Output layer with Softmax activation for 3 classes (BCC, SK, AK).
Image processing:
- Images resized to 600x600 pixels.
- Applied EfficientNet preprocessing and normalization.
- Used data augumentation (rotation, zoom flipping) to improve generalization.
Training Techniques- 
- Early stopping was used to prevent overfitting.
- ModelCheckpoint to save the best model.

Why we used EfficientNetB1 model?
- EfficientNetB1 provides high accuracy with fewer parameters, making it efficient for image classification tasks
- The model is pretrained on ImageNet, allowing effective transfer learning for medical image dataset
- EfficientNet architectures are known to perform well in medical image classification tasks
- It helps capture fine visual features in skin lesion images, which is important for detecting cancer patterns

Models weight could not be added bcz of Limitation of size in Github.

Results:

The trained model achieved approximately:

Accuracy: 78%
Precision: 79%
Recall: 78%
F1 Score: 78%
Model performance was evaluated using standard classification metrics and visualized through training accuracy and loss graphs.

Technologies Used:
- Python
- Tensorflow/ keras
- NumPy
- OpenCV
- Matplotlib
- Scikit-learn


Author

Sairaj Jagtap

B.Tech Computer Science (Artificial Intelligence & Machine Learning)

Sanjivani University






