Caltech101 Image Classification Project

Introduction
Welcome to the Caltech101 Image Classification Project! In this project, we classify images from the renowned Caltech101 dataset using three different machine learning algorithms: Nearest Neighbor, Neural Network, and Support Vector Machine (SVM). The dataset includes images from 101 diverse classes such as airplanes, cameras, and elephants. Instead of working directly with the image data, we utilize an extracted feature known as the Edge Histogram.

Dataset Description
Images.csv
This file contains the image IDs and their corresponding class labels. The first line indicates the number of images, and each subsequent line contains an image ID and a class separated by a semicolon.

Example:

Copy code
3
1;airplanes
32;beaver
454;chair
EdgeHistogram.csv
This file contains the feature vectors for the Edge Histogram feature. The first line contains the number of images followed by the number of dimensions, separated by a semicolon. Each subsequent line contains an image ID followed by the feature vector, with all values separated by semicolons.

Example:

Copy code
3;4
1;12;32;44;8
32;69;89;11;42
454;130;22;45;76
Results
After implementing and fine-tuning the three algorithms, we achieved the following highest accuracies:

Support Vector Machine (SVM): 59.60%
Neural Network: 52.65%
Nearest Neighbor: 49.21%
Methods
Data Preparation
Combining Data: Merge Images.csv and EdgeHistogram.csv using the image ID as the primary key.
Splitting Data: Divide the combined data into training (TR) and testing (TE) sets using a suitable ratio.
Algorithms Implemented
Nearest Neighbor
Neural Network
Support Vector Machine (SVM)
Hyperparameter Tuning
Fine-tuning hyperparameters for each algorithm to achieve optimal performance.

Installation
To run this project, ensure you have the required Python libraries installed. Use the following commands to install them:

bash
Copy code
pip install pandas
pip install numpy
pip install tensorflow
pip install scikit-learn
Experiment Setup
Data Loading and Preprocessing: Load the Images.csv and EdgeHistogram.csv files, preprocess them, and join them on the image ID.
Data Splitting: Split the data into training and testing sets.
Model Training: Train the Nearest Neighbor, Neural Network, and SVM models using the training data.
Hyperparameter Tuning: Tune the hyperparameters for each model to optimize performance.
Evaluation: Evaluate the models on the testing data and record the accuracies.
Conclusion
This project demonstrates the application of Nearest Neighbor, Neural Network, and Support Vector Machine algorithms to the Caltech101 dataset using Edge Histogram features. The SVM algorithm achieved the highest accuracy of 59.60%, followed by the Neural Network with 52.65%, and the Nearest Neighbor with 49.21%.

Output Files
