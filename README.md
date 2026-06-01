# Intelligent Crop Disease Detection using ANN 🌾🤖

This repository contains the official implementation of the **Intelligent Crop Disease Detection** system, developed as a lab project for the BS(AI) 5th Semester. The project utilizes an **Artificial Neural Network (ANN)** to classify crop health conditions and is deployed via a **Flask web application**.

## 📌 Project Overview
Traditional manual crop inspection is time-consuming and prone to errors. This system provides an automated, efficient approach by analyzing agricultural indicators and crop dataset features to detect conditions like **Leaf Blight, Rust, Early Blight, and Leaf Spot**.

## 📊 Dataset & Features
The model is aligned with the proposed architectural design, simulating a structured agricultural dataset containing key variables:
- **Numerical Features:** Temperature, Humidity, Soil Moisture, Leaf Color Index, Texture Score.
- **Categorical Targets:** Class labels representing specific plant conditions (e.g., Healthy, Leaf Blight, Rust).

## 🧠 Model Architecture (ANN)
Built using **TensorFlow/Keras**, the sequential model consists of:
1. **Flatten Layer:** Reshapes the input structural shape into a 1D vector.
2. **Hidden Layer 1:** Dense layer with 64 units and `ReLU` activation.
3. **Hidden Layer 2:** Dense layer with 32 units and `ReLU` activation.
4. **Output Layer:** Dense layer with a `Softmax` classifier matching the total number of target classes.

### Hyperparameters:
- **Optimizer:** Adam
- **Loss Function:** Sparse Categorical Cross-Entropy
- **Batch Size:** 32

## 🚀 Web Deployment (Flask App)
The system integrates a live interactive web UI where agricultural samples or images can be uploaded. The background Flask server triggers the pipeline to output the real-time detection status instantly.

## 🛠️ Tools & Technologies Used
- **Language:** Python
- **Frameworks:** TensorFlow, Keras, Flask
- **Libraries:** Pandas, NumPy, Scikit-learn
- **Environment:** Google Colab / Jupyter Notebook

## 👨‍💻 Author
- **Student Name:** Danyal Nasir Janjua
- **Registration Number:** 23108340
- **Department:** Robotics & Artificial Intelligence, SZABIST Islamabad
- **Submitted To:** Sir Hassan Mujtaba
