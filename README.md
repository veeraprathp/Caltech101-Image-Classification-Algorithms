  # Caltech101 Image Classification Project

## Introduction

This project involves classifying images from the Caltech101 dataset using three different machine learning algorithms: Nearest Neighbor, Neural Network, and Support Vector Machine (SVM). The dataset includes images from 101 different classes such as airplanes, cameras, and elephants. Instead of working directly with the image data, we use an already extracted feature called Edge Histogram.

The dataset consists of two files:
- `Images.csv`: Contains image IDs and their corresponding classes.
- `EdgeHistogram.csv`: Contains the feature data for the Edge Histogram feature for the images.

The two files are joined using the image ID as the primary key.

## Dataset Description

### Images.csv
Contains the image IDs and their corresponding class labels. The first line indicates the number of images. Each subsequent line contains an image ID and a class separated by a semicolon.



### EdgeHistogram.csv
Contains the feature vectors for the Edge Histogram feature. The first line contains the number of images followed by the number of dimensions separated by a semicolon. Each subsequent line contains an image ID followed by the feature vector, with all values separated by semicolons.



## Results

After implementing and fine-tuning the three algorithms, the highest accuracies achieved are as follows:

- **Support Vector Machine (SVM)**: 0.5959540732640787
- **Neural Network**: 0.5265172225259704
- **Nearest Neighbor**: 0.4920721705850191

## Methods

### Data Preparation
1. Combine `Images.csv` and `EdgeHistogram.csv` using the image ID as the primary key.
2. Split the combined data into training (TR) and testing (TE) sets using an appropriate ratio.

### Algorithms Implemented
- **Nearest Neighbor**
- **Neural Network**
- **Support Vector Machine (SVM)**

### Hyperparameter Tuning
For each algorithm, hyperparameters were fine-tuned to achieve the highest accuracy.

## Installation

To run this project, ensure you have the required Python libraries installed. Use the following commands to install them:

```bash
pip install pandas
pip install numpy
pip install tensorflow
pip install scikit-learn
