**Introduction-to-machine-learning---Final-Project---TM-NZS-**
Final project for the Introduction to Machine Learning course created by Téglás Máté (FWQPSP) and Németh Zsombor (HV911G).

Project Description

Our chosen project is Project 20: Gender and Age Prediction Based on Facial Images.

The goal of this project is to develop deep learning models capable of extracting demographic information from facial images. Specifically, we investigate how Convolutional Neural Networks (CNNs) can be used to predict a person’s gender and age from a single image.

The project consists of two main tasks:

1. Gender Classification

A binary image classification model was developed to determine whether a person in a facial image is male or female.

The model was trained using a CNN architecture consisting of multiple convolutional and pooling layers followed by fully connected layers. Images were resized to 256 × 256 pixels, normalized, and organized into training and validation datasets using TensorFlow’s data pipeline.

The model was trained for 10 epochs and evaluated using:

* Classification accuracy
* Confusion matrix
* Classification report (precision, recall, F1-score)

2. Age and Gender Prediction

A second, more advanced CNN model was developed using the UTKFace dataset. This model performs two tasks simultaneously:

* Gender classification
* Age prediction

The network uses a shared convolutional feature extractor and two separate output branches:

* A classification branch for gender prediction
* A regression branch for age estimation

This multi-output architecture allows the model to learn common facial features while optimizing separately for each prediction task.

Data augmentation techniques such as random flipping, rotation, zooming, and brightness adjustment were applied to improve generalization and reduce overfitting.

The model was evaluated using:

* Gender classification accuracy
* Mean Absolute Error (MAE) for age prediction
* Loss curves and training history
* Error distribution analysis
* Predicted versus true age comparisons

Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

Dataset

The project uses facial image datasets stored on Google Drive and the UTKFace dataset for age and gender prediction. The datasets are divided into training, validation, and testing subsets to ensure reliable model evaluation.

Results

The trained models demonstrate that CNNs can successfully learn facial features relevant for demographic prediction. The gender classifier achieves high classification performance, while the multi-output model is capable of estimating age and gender simultaneously from a single facial image.

The project highlights both the capabilities and limitations of deep learning approaches for facial attribute prediction and provides a practical application of convolutional neural networks in computer vision.
