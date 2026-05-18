🩺 Diabetes Prediction API – End-to-End MLOps Project

An end-to-end Machine Learning Operations (MLOps) project that predicts whether a patient is likely to have diabetes based on key health indicators. This project demonstrates the complete ML lifecycle, from model training to production deployment using modern DevOps and cloud-native tools.

🚀 Project Overview

This project was built to gain hands-on experience with practical MLOps concepts, including:

Data ingestion and preprocessing
Model training using a supervised learning algorithm
Model serialization and artifact management
REST API development for model inference
Containerization for reproducible deployments
Kubernetes-based orchestration

The goal was to understand not only how to build a machine learning model, but also how to package, deploy, and serve it in a scalable and production-oriented manner.

📊 Problem Statement

The application predicts whether a person is diabetic using the following features:

Pregnancies
Glucose
Blood Pressure
Body Mass Index (BMI)
Age

The model is trained on the Pima Indians Diabetes dataset and returns a binary prediction indicating whether the patient is likely to have diabetes.

🏗️ Architecture

Dataset → Data Preprocessing → Model Training → Serialized Model Artifact → FastAPI Inference Service → Docker Container → Kubernetes Deployment

🛠️ Technology Stack
Python
Pandas
NumPy
Scikit-learn
FastAPI
Pydantic
Joblib
Docker
Kubernetes
📁 Project Structure
train.py – Loads the dataset, trains the model, and saves the serialized artifact
main.py – Exposes prediction endpoints through a FastAPI application
diabetes_model.pkl – Trained model artifact
requirements.txt – Python dependencies
Dockerfile – Container build instructions
k8s-deploy.yml – Kubernetes deployment manifest
.gitignore
README.md
⚙️ Workflow
1. Data Preparation

The dataset is loaded from a public source and relevant features are selected for model training.

2. Model Training

A Random Forest Classifier is trained on the prepared data.

3. Model Serialization

The trained model is saved using Joblib for reuse during inference.

4. API Development

A FastAPI service loads the serialized model and exposes REST endpoints for predictions.

5. Containerization

The application is packaged into a Docker container to ensure portability and consistency across environments.

6. Kubernetes Deployment

The containerized application is deployed to Kubernetes for scalable and resilient serving.

📥 API Input Features

The prediction API accepts the following inputs:

Pregnancies
Glucose
BloodPressure
BMI
Age
Sample Output
{
  "diabetic": true
}
📌 Key Learnings

Through this project, I gained practical experience in:

Converting a trained machine learning model into a production-ready API
Designing input validation using typed schemas
Packaging applications with Docker
Deploying and managing workloads in Kubernetes
Structuring ML projects using MLOps best practices

This project helped me understand how machine learning, backend engineering, and cloud infrastructure come together to deliver scalable AI solutions.

🚀 Future Enhancements

Planned improvements include:

Model evaluation metrics and experiment tracking
CI/CD automation
Model versioning with MLflow
Logging and monitoring
Unit and integration tests
Cloud deployment on AWS
💡 Motivation

I built this project to explore the operational side of machine learning. While developing accurate models is important, deploying them in a reliable and scalable way is what makes them useful in real-world applications. This project gave me hands-on exposure to the engineering practices required to productionize machine learning systems.