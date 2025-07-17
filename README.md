
# K-Nearest Neighbors (KNN) and Radius Neighbors (RNN) Classifiers on the Wine Dataset

## Overview

In this lab, we explored the performance of **K-Nearest Neighbors (KNN)** and **Radius Neighbors (RNN)** classifiers using the **Wine Dataset** from the `sklearn` Python library. The dataset consists of three classes of wine with various chemical properties as features. By applying both KNN and RNN models, we analyzed the impact of different parameter values on model accuracy and visualized the key results. This exercise helps to understand how parameter choices influence classification performance and guides the selection of optimal values.

## Lab Instructions

### Step 1: Load and Prepare the Dataset
- **Dataset**: The Wine dataset includes 13 features, such as chemical properties of wine, that classify the wines into three classes (`class_0`, `class_1`, and `class_2`).
- **Data Split**: The dataset is split into **80% training** and **20% testing** sets to train the models and evaluate their performance.

### Step 2: Implement K-Nearest Neighbors (KNN)
- The **KNN Classifier** is applied using various values of `k` (1, 5, 11, 15, and 21). The model is trained on the training set, and accuracy is evaluated on the test set for each `k` value.

### Step 3: Implement Radius Neighbors (RNN)
- The **RNN Classifier** is applied using different radius values (350, 400, 450, 500, 550, and 600). The model is trained on the training set, and accuracy is evaluated on the test set for each radius value.

### Step 4: Visualize and Compare Results
- **Visualization**: The accuracy trends for both KNN (`k` values) and RNN (`radius` values) are plotted. The graphs show how the accuracy of each classifier changes with different parameter settings.

### Step 5: Comparison and Conclusion
- **Best Accuracy**: The highest accuracy for each classifier is determined, and the best values for `k` and `radius` are printed.
- **Conclusion**: A comparison is made between the performance of KNN and RNN, and observations are made on when each model might be preferable based on the results.

## Dataset Details

- **Dataset Features**:  
  The dataset includes the following chemical features of wine:
  - `'alcohol'`
  - `'malic_acid'`
  - `'ash'`
  - `'alcalinity_of_ash'`
  - `'magnesium'`
  - `'total_phenols'`
  - `'flavanoids'`
  - `'nonflavanoid_phenols'`
  - `'proanthocyanins'`
  - `'color_intensity'`
  - `'hue'`
  - `'od280/od315_of_diluted_wines'`
  - `'proline'`

- **Dataset Classes**:  
  The dataset contains three classes of wine:
  - `class_0`
  - `class_1`
  - `class_2`

- **Class Distribution**:  
  The class distribution in the dataset is as follows:
  - **Class 0**: 59 samples
  - **Class 1**: 71 samples
  - **Class 2**: 48 samples

## Results

- **Best KNN Accuracy**:  
  The best accuracy achieved by the KNN classifier was **77.78%** with `k = 1`.

- **Best RNN Accuracy**:  
  The best accuracy achieved by the RNN classifier was **75.00%** with a `radius = 350`.

## Conclusion

- The KNN model performed slightly better than the RNN model for this dataset, with the highest accuracy achieved at `k = 1`.
- The RNN model's performance was also good, with the best results at a radius value of **350**.
- The choice between KNN and RNN depends on the nature of the dataset. KNN might be preferable when the dataset is dense and the number of neighbors is well-defined, while RNN might be better suited when the data points have varying density and require a flexible radius to determine neighbors.
