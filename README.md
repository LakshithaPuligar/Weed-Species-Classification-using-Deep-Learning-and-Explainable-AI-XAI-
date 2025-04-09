# Weed-Species-Classification-using-Deep-Learning-and-Explainable-AI-XAI-
This project focuses on building a robust deep learning model to classify various weed species from the DeepWeed dataset. The model not only achieves high accuracy but also incorporates explainability through Grad-CAM heatmaps to visually interpret model predictions. 

Creating a convolutional neural network (CNN) to categorize different types of weeds.

For accuracy and efficiency, use MobileNetV2 with transfer learning.

Create heatmaps using Grad-CAM (Gradient-weighted Class Activation Mapping) to display the aspects of an image that affected the model's predictions.

Make sure the model is reliable and comprehensible for practical application in agricultural environments.

ABOUT THE DATASET-:
The DeepWeed dataset is a publicly available collection of weed images captured from agricultural fields in Australia. It includes:

17,509 images

9 classes (8 weed species + 1 negative class)

Images taken in diverse environmental conditions

Classes:
Chinee Apple

Lantana

Parkinsonia

Parthenium

Prickly Acacia

Rubber Vine

Siam Weed

Snake Weed

Negative (non-weed)

Base Model: MobileNetV2 (pre-trained on ImageNet, include_top=False)

Custom Layers:

Global Average Pooling

Dense layer with ReLU activation

Final Dense layer with Softmax for multi-class classification

Hyperparameters:
Image Size: 224x224

Optimizer: Adam

Loss Function: Categorical Crossentropy

Epochs: 5–20 (tuned based on performance)

Data Split: 80% train, 10% validation, 10% test

Accuracy	~92%
To interpret predictions, Grad-CAM is applied to visualize the most influential regions in each image that contributed to the predicted class.
These heatmaps:

Improve model transparency

Assist researchers and farmers in understanding model decisions


