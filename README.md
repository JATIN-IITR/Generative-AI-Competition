# Generative-AI-Competition
Detect the AI-generated photos - AI Generated Image Binary Classifier

# AI Generated Image Binary Classifier

This project is a binary classifier designed to detect AI-generated images. The classifier is implemented using the Adaboost algorithm from the Scikit-learn library. The models used for classification include DecisionTreeClassifier as the base classifier, and various models from the Torchvision library, namely ResNet18, ResNet50, VGG16, ConvNext, and Vision Transformer.

## Parameters

### Adaboost Classifier
- Base Classifier: DecisionTreeClassifier
  - Maximum Depth: 3
- Number of Estimators: 50
- Learning Rate: 1.0

### Torchvision Models
The following models from the Torchvision library were used for classification:

1. ResNet18
2. ResNet50
3. VGG16
4. ConvNext
5. Vision Transformer

For each model, the following parameters were used:

- Optimizer: AdamW
- Learning Rate: 0.001

## Data

The training and testing data used in this project are provided in CSV (Comma-Separated Values) file format. Prior to training the models, the data was preprocessed using the following steps:

1. Scaling: The data was scaled using the MinMaxScaler. This transformation brings the feature values within a specific range (usually between 0 and 1) to ensure compatibility with the models.
2. Principal Component Analysis (PCA): PCA was applied to the scaled data, reducing the dimensionality of the dataset. It was performed with 200 components, which helps to capture the most important patterns and variations in the data.

## Usage

To use this binary classifier, follow these steps:

1. Ensure that you have the necessary dependencies installed. The required libraries are Scikit-learn and Torchvision.
2. Prepare your training and testing data in CSV format.
3. Scale your data using the MinMaxScaler. Make sure to scale both the training and testing datasets.
4. Apply PCA with 200 components to the scaled data.
5. Instantiate the Adaboost classifier with the specified parameters.
6. Fit the classifier to the training data.
7. Evaluate the performance of the classifier on the testing data.


## Conclusion

This readme file provides an overview of the AI Generated Image Binary Classifier. It explains the parameters used for the Adaboost classifier and the Torchvision models. Additionally, it describes the data preprocessing steps, including scaling using MinMaxScaler and dimensionality reduction using PCA.

