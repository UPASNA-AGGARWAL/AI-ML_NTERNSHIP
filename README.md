# DRIVER DROWSINESS DETECTION

# Overview:
This project focuses on real-time detection of driver drowsiness using deep learning techniques, aiming to enhance road safety by alerting drivers proactively.
Key Features:

# TEST ACCURACY : 92.6%

<img width="892" alt="Screenshot 2024-06-19 at 10 47 25 AM" src="https://github.com/UPASNA-AGGARWAL/DRIVER_DROWSINESS/assets/120074587/87906e44-e60a-46b3-afc0-ac4e05919fed">

# Data Preprocessing and Augmentation:
Data undergoes preprocessing to enhance model robustness.
Augmentation techniques are applied to increase dataset diversity and improve model generalization.
Utilization of CNN (VGG16):
Advanced Convolutional Neural Network (CNN) architecture, specifically VGG16, is employed for feature extraction.
Visualization of Model Behavior:
Intermediate activations are visualized to gain insights into how the model processes information.
This visualization aids in understanding which features the model focuses on during drowsiness detection.
Model Training and Evaluation:
The model achieves high accuracy of 92.6% on the test dataset, demonstrating its effectiveness in detecting drowsiness.
Contribution to Road Safety:
The project contributes significantly to road safety by potentially preventing accidents caused by driver drowsiness.


# Training Data:
Total of 2467 training images with dimensions of 100 x 100 x 3 pixels.
Class distribution: {0: 617, 1: 617, 2: 616, 3: 617}
Test Data:
433 test images with similar dimensions.
Class distribution: {0: 109, 1: 106, 2: 109, 3: 109}
Image Statistics:
Mean and standard deviation are calculated for each color channel (Red, Green, Blue) to understand pixel value distributions.

# Data Augmentation:
An ImageDataGenerator is configured with parameters like rotation, shift, shear, zoom, and flip to augment the training images.
Augmentation helps in increasing dataset size and model robustness against variations in input images.

<img width="901" alt="Screenshot 2024-06-19 at 10 49 04 AM" src="https://github.com/UPASNA-AGGARWAL/DRIVER_DROWSINESS/assets/120074587/ee1b1d17-51dd-4914-b4c6-d39f999e3817">

# Model Architecture:
# Loading Pre-trained VGG16 Model:
The VGG16 model pre-trained on ImageNet is loaded, excluding the top classification layer.
Customization with Additional Layers:
Additional layers (Flatten and Dense) are added to adapt the VGG16 model for the specific drowsiness classification task.
The final layer uses a softmax activation function to classify images into drowsiness categories.

# Utilization of CNN Architectures:
The project employs the VGG16 architecture, pretrained on ImageNet, for feature extraction.
The VGG16 model is adapted by adding custom layers including Flatten and Dense with softmax activation for classification.

# Visualization of Model Behavior:
Intermediate activations of the VGG16 model are visualized to understand its behavior.
Activations from specific layers are extracted and displayed using matplotlib, aiding in model interpretation and debugging.

<img width="880" alt="Screenshot 2024-06-19 at 10 49 40 AM" src="https://github.com/UPASNA-AGGARWAL/DRIVER_DROWSINESS/assets/120074587/32992604-b71c-4ec3-93f4-8f5a6a13e8c9">


ChatGPT
Driver Drowsiness Detection Project Report

Overview:
This project focuses on real-time detection of driver drowsiness using deep learning techniques. Its primary objective is to enhance road safety by alerting drivers when signs of drowsiness are detected.

Key Features:

Data Preprocessing and Augmentation:

Data undergoes preprocessing and augmentation to improve model robustness.
Image data dimensions are standardized to 100 x 100 pixels with 3 color channels (RGB).
Mean pixel value across all channels is approximately 106.96, with a standard deviation of 68.82.
Channel-specific statistics: Channel 1 (mean: 120.20, std dev: 70.58), Channel 2 (mean: 104.27, std dev: 67.02), Channel 3 (mean: 96.40, std dev: 66.64).
Utilization of CNN Architectures:

The project employs the VGG16 architecture, pretrained on ImageNet, for feature extraction.
The VGG16 model is adapted by adding custom layers including Flatten and Dense with softmax activation for classification.
Model Training and Evaluation:

High accuracy of 92.6% is achieved on the test dataset.
Class distribution in training and test sets is balanced across four categories: {0, 1, 2, 3}.
Visualization of Model Behavior:

Intermediate activations of the VGG16 model are visualized to understand its behavior.
Activations from specific layers are extracted and displayed using matplotlib, aiding in model interpretation and debugging.
Contribution to Road Safety:

The project significantly contributes to road safety by providing early warning to drivers exhibiting signs of drowsiness, potentially preventing accidents.

ImageDataGenerator Configuration:
Augmentation parameters include rotation, width and height shifts, shear, zoom, and horizontal flip.

<img width="866" alt="Screenshot 2024-06-19 at 10 48 08 AM" src="https://github.com/UPASNA-AGGARWAL/DRIVER_DROWSINESS/assets/120074587/01a59d63-caf5-49e9-a49c-4a866799d7f9">

# CONCLUSION
This project effectively harnesses deep learning and computer vision techniques to address driver safety concerns associated with drowsiness. By leveraging advanced CNN architectures, robust data preprocessing, and insightful model visualization techniques, it achieves high detection accuracy and provides a crucial tool for enhancing road safety through early drowsiness detection and alert systems. The project’s methodologies and outcomes underscore its potential impact in reducing accidents and promoting safer driving practices.
