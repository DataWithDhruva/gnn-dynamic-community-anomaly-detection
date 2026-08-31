# GNN-Based Dynamic Community Anomaly Detection in Fraud Networks

A Graph Neural Network (GNN)-based approach for detecting anomalous or potentially fraudulent patterns in graph-structured networks.

## 📌 Project Overview

Fraudulent activities often involve relationships between multiple entities rather than isolated transactions. Traditional machine learning methods generally treat records independently, which can make it difficult to capture the relationships and structural patterns present in fraud networks.

This project investigates a graph-based approach for anomaly detection by representing entities and their relationships as a graph and applying Graph Neural Network techniques to learn meaningful node representations.

The project compares Graph Neural Network models with traditional machine learning approaches to evaluate their effectiveness in detecting anomalous patterns.

---

## 🎯 Objectives

* Represent fraud-related data as a graph.
* Capture relationships between connected entities.
* Apply Graph Neural Network techniques for anomaly detection.
* Implement and evaluate GraphSAGE-based models.
* Compare GNN models with traditional machine learning algorithms.
* Evaluate models using Precision, Recall, F1-score and ROC-AUC.
* Identify the model that provides the most effective fraud/anomaly detection performance.

---

## 🧠 Methodology

The overall workflow of the project is:

```text
Data Collection
      ↓
Data Preprocessing
      ↓
Graph Construction
      ↓
Exploratory Data Analysis
      ↓
Feature Preparation
      ↓
Graph Representation
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Model Comparison
      ↓
Final Analysis
```

---

## 🤖 Models Used

### Graph Neural Network Models

* GraphSAGE
* GraphSAGE with Focal Loss
* GCN (Graph Convolutional Network)
* GAT (Graph Attention Network)

### Traditional Machine Learning Models

* Logistic Regression
* Random Forest
* Gradient Boosting
* XGBoost

The traditional machine learning models are used as baseline models for comparison with graph-based approaches.

---

## 🛠️ Technologies & Tools

* Python
* PyTorch
* PyTorch Geometric
* NetworkX
* GraphSAGE
* Scikit-learn
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook

---

## 📊 Evaluation Metrics

The models are evaluated using:

* Precision
* Recall
* F1-Score
* ROC-AUC

These metrics help evaluate the models from different perspectives, particularly because fraud/anomaly detection can involve imbalanced classes.

---

## 📁 Dataset

The project uses benchmark/public and synthetic graph datasets for experimentation.

Datasets explored/used during the project include:

* Cora
* Public/Synthetic datasets
* Elliptic Bitcoin Dataset

Dataset files are not necessarily included directly in this repository when redistribution or repository-size limitations apply.

Refer to `data/README.md` for dataset information and preparation instructions.

---

## 📈 Results

The project evaluates multiple machine learning and graph neural network models using the selected evaluation metrics.

The experiments include:

| Model                  | Precision | Recall | F1-Score | ROC-AUC |
| ---------------------- | --------: | -----: | -------: | ------: |
| Logistic Regression    |         - |      - |        - |       - |
| Random Forest          |         - |      - |        - |       - |
| Gradient Boosting      |         - |      - |        - |       - |
| XGBoost                |         - |      - |        - |       - |
| GCN                    |         - |      - |        - |       - |
| GAT                    |         - |      - |        - |       - |
| GraphSAGE              |         - |      - |        - |       - |
| GraphSAGE + Focal Loss |         - |      - |        - |       - |

> Final experimental values will be added after completing and verifying the final evaluation.

### Best Performing Models

* **Best Test F1-Score:** Random Forest
* **Best Test ROC-AUC:** XGBoost

The results demonstrate that model performance depends on the evaluation metric and that traditional machine learning models can remain competitive against graph-based approaches under certain experimental settings.

---

## 🏗️ Project Architecture

```text
                ┌────────────────────┐
                │      Dataset       │
                └─────────┬──────────┘
                          ↓
                ┌────────────────────┐
                │ Data Preprocessing │
                └─────────┬──────────┘
                          ↓
                ┌────────────────────┐
                │ Graph Construction │
                └─────────┬──────────┘
                          ↓
                ┌────────────────────┐
                │ Feature Extraction │
                └─────────┬──────────┘
                          ↓
              ┌────────────────────────┐
              │   Model Training       │
              │                        │
              │ GCN | GAT | GraphSAGE │
              │ RF | XGB | LR | GB    │
              └───────────┬────────────┘
                          ↓
                ┌────────────────────┐
                │    Evaluation      │
                └─────────┬──────────┘
                          ↓
                ┌────────────────────┐
                │ Model Comparison   │
                └────────────────────┘
```

---

## 📂 Repository Structure

```text
├── data/
│   ├── raw/
│   ├── processed/
│   └── README.md
│
├── notebooks/
│   ├── data_preprocessing.ipynb
│   ├── exploratory_analysis.ipynb
│   └── model_training.ipynb
│
├── src/
│   ├── preprocessing/
│   ├── models/
│   ├── training/
│   ├── evaluation/
│   └── utils/
│
├── models/
├── results/
│   ├── figures/
│   └── metrics/
│
├── docs/
│   ├── project_report.pdf
│   ├── synopsis.pdf
│   └── presentation.pdf
│
├── requirements.txt
├── .gitignore
├── LICENSE
└── README.md
```

---

## 🚫 Project Scope & Limitations

The current project focuses on graph-based anomaly/fraud detection using experimental benchmark/public datasets.

The following components are outside the current project scope:

* Real-time fraud detection
* Real-time streaming data
* Time-evolving dynamic graph processing
* Reinforcement Learning components

---

## 🔬 Experimental Approach

The project follows an iterative experimental workflow:

1. Dataset preparation
2. Data preprocessing
3. Graph construction
4. Feature preparation
5. Baseline model implementation
6. GNN model implementation
7. Model training
8. Hyperparameter experimentation
9. Model evaluation
10. Performance comparison

---

## 👥 Team Members

**Group 14**

* Abhirup Bag
* Abhrajit Rath
* Arnab Chattopadhyay
* Dhruba Dey

---

## 🎓 Academic Project

**Final Year Project**
B.Tech in Computer Science and Engineering
Techno Main Salt Lake
Affiliated to MAKAUT

---

## 📌 Future Scope

Possible future improvements include:

* Real-time fraud detection
* Temporal/dynamic graph modelling
* Larger real-world fraud datasets
* Advanced GNN architectures
* Improved handling of highly imbalanced data
* Explainable Graph Neural Networks
* Real-time graph-based anomaly monitoring

---

## 📚 References

Relevant research papers, datasets, libraries and documentation used during the project will be listed here.

---

## 📄 Project Documentation

Project documentation will be maintained under the `docs/` directory.

This may include:

* Project Synopsis
* Final Project Report
* Presentation
* Supporting documentation

---

## ⭐ Acknowledgement

This project was developed as part of the Final Year Project requirement for the B.Tech in Computer Science and Engineering program.

---

## 📜 License

This project is intended for academic and educational purposes.
