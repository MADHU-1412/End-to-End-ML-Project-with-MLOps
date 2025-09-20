# **End-to-End Machine Learning Pipeline with MLOps**

## **Project Overview**

This project demonstrates a **complete machine learning workflow** from raw data preprocessing to model training, evaluation, and production deployment. It focuses on **MLOps principles**, including reproducible pipelines, Docker containerization, CI/CD automation with GitHub Actions, and deployment on AWS.

---

## **Features**

* Automated data preprocessing: missing value handling, categorical encoding, and numerical scaling.
* Model training and evaluation using scikit-learn pipelines.
* Serialization of the trained model for inference.
* Dockerized application for consistent deployment.
* CI/CD workflow using GitHub Actions for automated testing and deployment.
* Deployment on AWS EC2 with a production-ready setup.

---

## **Project Structure**

```
├── data/                # Raw and processed datasets
├── src/                 # Modular scripts for preprocessing, training, and prediction
├── models/              # Saved trained models
├── Dockerfile           # Docker configuration
├── requirements.txt     # Python dependencies
├── .github/workflows/   # CI/CD pipeline scripts
└── README.md
```

---

## **Technologies Used**

* **Languages:** Python
* **Libraries:** Pandas, NumPy, scikit-learn, joblib
* **Deployment & MLOps:** Docker, AWS EC2, AWS ECR, GitHub Actions

---

## **Getting Started**

### **Prerequisites**

* Python 3.8+
* Docker
* AWS account (for deployment)

### **Install Dependencies**

```bash
pip install -r requirements.txt
```

### **Run Locally**

1. Preprocess data and train model:

```bash
python src/train.py
```

2. Run predictions on new data:

```bash
python src/predict.py
```

### **Docker Deployment**

1. Build Docker image:

```bash
docker build -t ml_pipeline .
```

2. Run container:

```bash
docker run -p 5000:5000 ml_pipeline
```

---

## **CI/CD Workflow**

* Any commit triggers automated **testing and deployment** through GitHub Actions.
* Ensures reproducibility and reliability of the deployed model.

---

## **Learning Outcomes**

* Designed **production-ready ML pipelines** using scikit-learn.
* Implemented **Docker-based deployment** and CI/CD automation.
* Learned best practices for **scalable, reproducible, and maintainable ML systems**.
