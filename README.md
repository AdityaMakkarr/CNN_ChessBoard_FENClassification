# Chess Position Recognition using CNN

A computer vision project that uses a Convolutional Neural Network (CNN) to identify chess pieces from chessboard images and reconstruct the corresponding board position.

## Project Overview

The pipeline:

1. Takes a 400×400 chessboard image.
2. Splits the board into 64 individual squares.
3. Classifies each square into one of 13 classes:
   - Empty square
   - 6 white pieces
   - 6 black pieces
4. Reconstructs the predicted chess position from the 64 classifications.

## Model

A lightweight CNN was selected after comparing multiple model architectures, input resolutions and image conditions.

The final model consists of:

- 1 convolutional layer with 4 filters
- 3×3 convolution kernel
- Max pooling
- Flatten layer
- 13-class Softmax output

The final model achieved 100% classification accuracy on the unseen test dataset.

## Experiments

Experiments investigated:

- CNN model capacity
- Convolution kernel size
- Input image resolution
- Gaussian noise
- Rotation
- Image darkening
- Gaussian blur
- Occlusion

## Dataset

Chess Positions dataset by Pavel Koryakin:

https://www.kaggle.com/datasets/koryakinp/chess-positions

The dataset contains 100,000 generated chessboard images, divided into 80,000 training and 20,000 testing images.

## Technologies

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Pillow

## Repository

The main notebook contains the complete preprocessing, model development, experimental evaluation and final model assessment.


