# Facial Expression Detection

This project implements facial expression detection using a simple machine learning model. It processes images to detect facial expressions and classifies them into different emotion categories. The project avoids using OpenCV and relies on `PIL` (Pillow) for image processing and `scikit-learn` for machine learning.

## Prerequisites

Ensure you have Python installed on your system. You also need the following Python packages:

- `Pillow` for image processing
- `scikit-learn` for machine learning
- `numpy` for numerical operations

You can install these dependencies using pip:

```bash
pip install pillow scikit-learn numpy

Dataset

The project uses a synthetic dataset for demonstration purposes. Replace the synthetic dataset with a real dataset of facial expressions for practical use. For real-world applications, you may consider datasets like FER-2013.

Project Structure

main.py: The main script for facial expression detection. It includes functions to:
Load and preprocess images
Train a machine learning model
Predict facial expressions
Handle exceptions related to file paths

Code Overview

load_synthetic_dataset(): Generates synthetic data for demonstration. Replace this with actual dataset loading.
train_classifier(X_train, y_train): Trains an SVM classifier using the provided dataset.
preprocess_image(image): Processes images by converting them to grayscale and resizing them to 48x48 pixels.
predict_emotion(model, image): Predicts the emotion of the provided image using the trained model.
main(image_path): Main function to load an image, predict its emotion, and handle errors related to file paths.
