# MNIST Handwritten Digit Classification using KNN

## Project Overview

This project demonstrates the use of the **k-Nearest Neighbors (KNN)** algorithm to classify handwritten digits from the well-known **MNIST dataset**. KNN is a simple, yet powerful classification algorithm that predicts a label based on the majority vote of the nearest neighbors. The goal of this project is to achieve high accuracy in recognizing digits (0-9) through an efficient and optimized implementation.

## Key Features

- **KNN Implementation from Scratch:** This project builds the KNN algorithm from the ground up without relying on any pre-built machine learning libraries, providing deep insights into how KNN works.
- **Distance Calculation using L2 Norm:** The Euclidean distance formula (L2 norm) is used to calculate the similarity between the input images.
- **Optimized KNN:** The algorithm is optimized by computing distances in an efficient manner to handle large datasets like MNIST.
- **Accuracy Calculation:** The model is evaluated using accuracy metrics, providing a direct measure of its performance on unseen data.
- **Visualization of Results:** Selected handwritten digits are displayed to visually validate predictions against actual labels.

## Technology Stack

- **Programming Language:** Python
- **Libraries:** `numpy`, `matplotlib`
- **Algorithm:** k-Nearest Neighbors (KNN)
- **Dataset:** MNIST (from CSV)

## Workflow

1. **Data Loading & Preprocessing**
   - Downloaded the MNIST dataset and parsed the training and test sets.
   - Split the data into training (59,000 examples) and validation sets (1,000 examples).
   - Prepared features (`X`) and labels (`Y`) for both the training and validation data.

2. **KNN Classification**
   - Calculated distances between the validation images and all training images using the **L2 norm**.
   - For each validation sample, identified the **k-nearest neighbors** and used a weighted voting scheme to predict the most likely digit.
   - Optimized the KNN algorithm to avoid redundant calculations.

3. **Model Evaluation**
   - The model was tested on the validation set to compute **accuracy** and assess how well the model performs.
   - Visualized one of the validation set images along with its predicted label to confirm accuracy visually.

4. **Performance Metrics**
   - Achieved an accuracy of *X*% for k=20 using L2 distance on the validation set.
   - Explored different values of `k` and norms (e.g., L1, L2) to identify the optimal configuration for this dataset.

## Visualizations

- **Validation Image Visualization:** A selected image from the validation set is shown with the corresponding predicted label.
- **Accuracy for Different `k` Values:** Plots showing accuracy trends for different values of `k`.

## How to Run This Project

1. Clone the repository and install the necessary dependencies:
   ```bash
   git clone <https://github.com/vamsi51080/Hand-Written-Digit-Recognition/>
   cd Hand-Written-Digit-Recognition/
   ```

2. Download the MNIST dataset and run the script to perform KNN classification:


3. You can visualize the prediction for a random sample from the validation set:
   ```python
   visualise(validation_inputs[114])
   ```

## Why This Project Stands Out

Handwritten digit recognition is a classic problem in computer vision and machine learning, providing valuable insight into the basics of classification algorithms. By implementing KNN from scratch, I demonstrated the ability to:

- Efficiently handle large datasets.
- Optimize machine learning algorithms for better performance.
- Work with key Python libraries and data science tools.
- Understand and apply core concepts of supervised learning.

## Future Improvements

- **Dimensionality Reduction:** Implementing PCA (Principal Component Analysis) to reduce the feature space, improving the speed of distance calculations.
- **Hyperparameter Tuning:** Exploring different values of `k` and distance metrics to further improve accuracy.
- **Real-time Digit Recognition:** Extending the project to use real-time handwritten digit input from users via a graphical interface.

