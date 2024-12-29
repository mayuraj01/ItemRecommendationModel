# ItemRecommendationModel
This project demonstrates a Fashion Recommendation System that suggests similar fashion images based on a selected input image. It leverages ResNet50, a powerful convolutional neural network (CNN), for feature extraction and utilizes the Nearest Neighbors algorithm to find and display the most visually similar images.

# Features
Deep Learning-Based Feature Extraction: Uses a pre-trained ResNet50 model with weights trained on ImageNet to extract meaningful features from images.
Efficient Similarity Search: Implements a Nearest Neighbors model with the Euclidean distance metric to retrieve similar images quickly and accurately.
Image Preprocessing: Handles resizing, normalization, and preprocessing of images for optimal performance with the ResNet50 model.
Visualization: Displays the recommended images in a clear, user-friendly layout using Matplotlib.

# Technologies Used
Python
TensorFlow/Keras: For deep learning and feature extraction.
Scikit-learn: For implementing Nearest Neighbors.
OpenCV: For image preprocessing (via Keras utilities).
Matplotlib: For visualizing recommended images.
Pickle: For storing and loading image features and filenames.

