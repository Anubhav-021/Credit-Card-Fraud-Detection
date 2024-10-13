# Credit Card Fraud Detection using Self-Organizing Maps (SOM)

This project demonstrates how to detect credit card fraud using a Self-Organizing Map (SOM). SOMs are a type of unsupervised neural network that can be useful for detecting patterns and anomalies in datasets, making them ideal for fraud detection tasks.

## Project Overview

Credit card fraud detection is a critical challenge in the financial industry. This project uses a dataset of credit card applications and applies a Self-Organizing Map to detect potential fraud by identifying unusual patterns in the data.

The SOM clusters the dataset into different groups based on their similarities and flags potential anomalies, which could indicate fraudulent applications.

## Features 

1. Unsupervised Learning with SOM: No labels are required, making it suitable for anomaly detection tasks.
2. Data Preprocessing: Includes feature scaling and preparation.
3. Visualization: The resulting SOM is visualized to highlight anomalies.

## Dataset

The dataset used in this project is Credit_Card_Applications.csv. It contains various features related to credit card applications, and the goal is to identify abnormal applications that may indicate fraudulent activity.

## How It Works

1. Data Loading and Preprocessing:
The dataset is loaded and split into feature variables (X) and labels (y).
Feature scaling is applied using MinMaxScaler to normalize the data.

2. Training the Self-Organizing Map:
A SOM is initialized with a 10x10 grid, and the training is performed on the dataset.
The SOM clusters the data points based on similarities in the input features.

3. Fraud Detection:
After training, the SOM identifies applications that do not fit well into the clusters as potential frauds.
These outliers are visualized for further analysis.

## How to Run the Project
1. Clone the repository:

```git clone https://github.com/yourusername/credit-card-fraud-detection-som.git
cd credit-card-fraud-detection-som
```

2. Run the Jupyter notebook to execute the code:

```jupyter notebook Hybrid_SOM.ipynb```

Follow the instructions in the notebook to preprocess the data, train the SOM, and visualize the results.

## Results

The Self-Organizing Map produces a grid where each node represents a cluster of similar applications. By analyzing the distances between the nodes, potential fraudulent credit card applications are highlighted.

## Visualization

The results are visualized using a Matplotlib plot that shows the clusters and highlights the potential outliers or anomalies.

## Technologies Used
1. Python
2. Pandas for data manipulation
3. NumPy for numerical operations
4. MiniSom for building and training the SOM
5. Matplotlib for visualization
6. Scikit-learn for data preprocessing

## Conclusion

This project demonstrates how SOMs can be used for unsupervised anomaly detection in credit card fraud detection. It can serve as a foundation for more complex fraud detection systems by combining unsupervised learning methods with domain-specific knowledge.
