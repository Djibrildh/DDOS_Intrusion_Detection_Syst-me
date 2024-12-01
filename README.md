# IDS Project - Intrusion Detection System

## **Project Overview**

As part of my studies in the Master’s program in Engineering and Artificial Intelligence at Université Paris 8, I developed this project to explore artificial intelligence learning techniques. The goal is to create an **Intrusion Detection System (IDS)** using machine learning methods. The primary objective is to detect anomalous behavior and potential DDoS attacks in a network using supervised (Random Forest, SVC) and unsupervised models (Autoencoder).

The dataset used is **CICIDS 2017**, which contains a variety of network traffic types, including benign behavior and DDoS attacks.


## **Objective**
1. Preprocess the data to handle missing values, scale features, and remove outliers.
2. Train and compare different models:
   - **Autoencoder** for unsupervised anomaly detection.
   - **Random Forest** and **SVC** for supervised classification.
3. Evaluate model performance with metrics like accuracy, F1-score, and AUC-ROC.

## **Project Structure**

- `data/`: Contains the CICIDS 2017 dataset files in CSV format.
- `models/`: Stores trained models (`.h5` for the autoencoder and `.pkl` for other models).
- `main_notebook.ipynb`: Main script to view the project.
- `README.md`: Project documentation.
- `requirements.txt` : contains all used libraries


## **Prerequisites**

- Python 3.9 or higher.
- A virtual environment is recommended (`venv` or `conda`).
- Required libraries (specified in `requirements.txt`).
- An IDE (Jupiter notebook, google collab ...)

## **Project Steps**
1. **Preprocessing:**
   - Handle missing values using median imputation.
   - Normalize data with MinMaxScaler.
   - Reduce dimensionality using PCA to retain 95% of the variance.

2. **Model Training:**
   - Train an autoencoder to identify reconstruction errors as anomalies.
   - Train Random Forest and SVC models on labeled data.

3. **Evaluation:**
   - Use metrics like accuracy, precision, recall, and F1-score.
   - Visualize results with ROC curves and reconstruction error distributions.


## **How to Run the Notebook**
1. Install dependencies:
`pip install -r requirements.txt` or `pip3 install -r requirements.txt`
2. Open the notebook in Jupyter or any compatible environment.
3. Follow the sections:
    - Preprocessing
    - Model Training
    - Evaluation

## **Key Results**
- **Autoencoder**: Demonstrated some ability to separate benign traffic from anomalies, but performance can be improved.
- **Random Forest and SVC**: Achieved high accuracy due to supervised learning but require balanced preprocessing for robustness.


## **Future Improvements**
- Explore better preprocessing techniques for handling outliers and scaling.
- Test more advanced models like Gradient Boosting or deep learning architectures (e.g., LSTMs).
- Expand the dataset to include other types of attacks for better generalization.


## Remerciment
Thank you for taking the time to read this README. I hope you find my work satisfactory.
#### Djibril DAHOUB 