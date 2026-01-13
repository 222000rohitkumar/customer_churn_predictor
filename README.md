This is a comprehensive, professional `README.md` content designed to cover every aspect of your project—from the technical architecture to the installation steps.

---

# 📊 Customer Churn Predictor: End-to-End Deep Learning Project

## 📌 Project Overview

The **Customer Churn Predictor** is a sophisticated data science application designed to help financial institutions identify customers who are likely to leave the bank. By leveraging an **Artificial Neural Network (ANN)**, the system analyzes historical customer behavior and provides a probability of churn, enabling proactive retention strategies.

This project covers the entire machine learning lifecycle: Data Cleaning, Feature Engineering, Model Building, Hyperparameter Tuning, and Deployment via a Web Interface.

---

## 🛠️ Key Features

* **Deep Learning Core:** Built with a Multi-Layer Perceptron (ANN) for high-accuracy classification.
* **Interactive UI:** A sleek Streamlit dashboard for real-time customer analysis.
* **Robust Preprocessing:** Handles categorical encoding (One-Hot & Label) and feature scaling automatically.
* **Optimization:** Includes hyperparameter tuning logs to show how the best model was achieved.
* **Salary Regression:** Includes an experimental branch for predicting estimated salaries.

---

## 📂 Repository Structure

| File | Description |
| --- | --- |
| `app.py` | The main Streamlit application script for the web UI. |
| `model.h5` | The final trained and saved Keras ANN model. |
| `Churn_Modelling.csv` | The raw dataset containing 10,000 customer records. |
| `experiments.ipynb` | Initial EDA, data visualization, and baseline model tests. |
| `hyperparametertuningann.ipynb` | Keras Tuner/GridSearch experiments for optimizing layers and neurons. |
| `scaler.pkl` | Serialized StandardScaler used to normalize input features. |
| `label_encoder_gender.pkl` | Transformer for converting Gender into numerical format. |
| `onehot_encoder_geo.pkl` | Transformer for Geography (France, Germany, Spain) encoding. |
| `requirements.txt` | List of all Python libraries required to run the project. |

---

## 🧠 Model Architecture

The underlying model is a **Feed-Forward Artificial Neural Network** with the following configuration:

1. **Input Layer:** Receives 11+ processed features.
2. **Hidden Layers:** Dense layers with **ReLU** activation and Dropout for regularization.
3. **Output Layer:** A single neuron with a **Sigmoid** activation function to output a churn probability (0 to 1).
4. **Optimizer:** Adam optimizer with Binary Cross-Entropy loss.

---

## 🚀 Getting Started

### 1. Prerequisites

Ensure you have Python 3.8+ installed on your machine.

### 2. Installation

Clone the repository and install the necessary dependencies:

```bash
# Clone the repo
git clone https://github.com/222000rohitkumar/customer_churn_predictor.git

# Navigate into the folder
cd customer_churn_predictor

# Create a virtual environment
python -m venv venv

# Activate venv
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate

# Install requirements
pip install -r requirements.txt

```

### 3. Running the App

Launch the Streamlit interface:

```bash
streamlit run app.py

```

The application will be available at `http://localhost:8501`.

---

## 📊 Data Features Used

The model predicts churn based on these specific inputs:

* **Credit Score:** Numeric score of the customer's creditworthiness.
* **Geography:** France, Spain, or Germany.
* **Gender:** Male or Female.
* **Age:** Age of the customer.
* **Tenure:** Number of years the customer has been with the bank.
* **Balance:** Current account balance.
* **Number of Products:** How many bank products the customer uses.
* **Has Credit Card:** Yes (1) or No (0).
* **Is Active Member:** Whether the customer is frequently active.
* **Estimated Salary:** Annual income of the customer.

---

## 🧪 Experiments & Tuning

For those interested in the research behind the model:

* Open `experiments.ipynb` to see the **Exploratory Data Analysis (EDA)**, including correlation heatmaps and churn distribution charts.
* Open `hyperparametertuningann.ipynb` to see how the number of neurons and learning rates were optimized to maximize the **F1-Score** and **Accuracy**.

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 👨‍💻 Author

**Rohit Kumar**

* GitHub: [@222000rohitkumar](https://www.google.com/search?q=https://github.com/222000rohitkumar)

---

*⭐ If you find this project useful, please consider giving it a star!*
