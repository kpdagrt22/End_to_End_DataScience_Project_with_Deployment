# End-to-End ML Project with MLOps | Modular, Trackable, and Deployable

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/93/Amazon_Web_Services_Logo.svg" alt="AWS" height="40"/>
  <img src="https://github.com/apache/airflow/blob/main/airflow-core/docs/img/logos/wordmark_1.svg?raw=true" alt="Airflow" height="40"/>
  <img src="https://avatars.githubusercontent.com/u/41825161?s=200&v=4" alt="DVC" height="40"/>
  <img src="https://github.com/mlflow/mlflow/blob/master/assets/logo.svg?raw=true" alt="MLflow" height="40"/>
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4e/Docker_%28container_engine%29_logo.svg" alt="Docker" height="40"/>
  <img src="https://commons.wikimedia.org/wiki/File:FastAPI_logo.svg#/media/File:FastAPI_logo.svg" alt="FastAPI" height="40"/>
  <img src="https://logowik.com/content/uploads/images/grafana3182.jpg" alt="Grafana" height="40"/>
</p>

## 🚀 Project Overview
This project demonstrates a **complete, production-ready data science workflow** implemented using **modular design principles**. It covers every stage of the ML lifecycle — from **data ingestion** to **model evaluation and tracking** — and adheres to **industry best practices** for configuration, pipeline orchestration, and experiment management.

---

## 📌 Features
- **Modular architecture** using Python packages and custom components
- **Version-controlled datasets and models** via DVC and Git
- **ML pipeline orchestration** using Apache Airflow & Astronomer
- **Experiment tracking** with MLflow
- **Deployment-ready app** using FastAPI
- **Monitoring with Grafana dashboards**
- **Config and schema management** with YAML
- **Automated folder and logging setup**

---

## 🧱 Project Architecture
```
project-root/
│
├── config/                  # YAML-based config files
├── constants/              # Hard-coded values and constants
├── entity/                 # Data classes for type safety
├── components/             # Core ML pipeline components
│   ├── data_ingestion.py
│   ├── data_transformation.py
│   ├── model_trainer.py
│   └── model_evaluation.py
│
├── pipeline/               # Training and prediction pipelines
│
├── utils/                  # Common reusable functions
│
├── logs/                   # Central logging location
├── templates/              # Flask/FastAPI HTML templates (for app)
├── Dockerfile              # Containerization setup
├── requirements.txt        # Dependencies
├── setup.py                # For packaging
├── main.py                 # Trigger pipeline execution
└── README.md
```

---

## ⚙️ Technologies Used
- **Languages & Libraries**: Python, Scikit-learn, Pandas, Matplotlib, YAML, Joblib
- **MLOps & Workflow**: MLflow, DVC, Apache Airflow, Astronomer
- **Deployment**: Docker, FastAPI
- **Cloud**: AWS EC2, S3
- **Monitoring**: Grafana
- **Utilities**: ConfigBox, Ensure Annotation, Logging, GitHub Actions

---

## 🧪 ML Lifecycle
1. **Data Ingestion**: Reads zipped data from GitHub, unzips & stores in `artifacts`
2. **Data Validation**: Validates schema using YAML
3. **Data Transformation**: Cleans and prepares features
4. **Model Training**: Trains a RandomForest model, logs with MLflow
5. **Model Evaluation**: Compares metrics, selects best model
6. **Deployment**: Docker + FastAPI endpoint ready for inference
7. **Monitoring**: Metrics tracked using MLflow UI and Grafana dashboards

---

## 📁 Configuration Strategy
All runtime parameters (e.g., file paths, model settings, schema) are defined in:
- `config.yaml`
- `params.yaml`
- `schema.yaml`

These are read using `ConfigBox` for dot-access and type safety.

---

## 🧰 How to Run
```bash
# Step 1: Create Conda environment
conda create -p venv python=3.10 -y
conda activate ./venv

# Step 2: Install dependencies
pip install -r requirements.txt

# Step 3: Set up and run project
python template.py     # auto-generates folder structure
python main.py         # runs the training pipeline

# Step 4: Track experiment
mlflow ui              # opens MLflow dashboard

# Optional: Deploy with Docker
docker build -t mlproject .
docker run -p 8080:8080 mlproject
```

---

## 👨‍💻 Author
**Prakash Kantumutchu**  
AI/ML Engineer | 7.5+ Yrs Experience  
[GitHub](https://github.com/kpdagrt22) | [LinkedIn](https://linkedin.com/in/prakash-kantumutchu)  

---

## 📌 Certifications Related to This Project
- AI Agent Developer — Vanderbilt University
- Azure AI Engineer Associate (AI-102)
- Machine Learning Scientist with Python — DataCamp
- Docker Foundations, GitHub Actions Pro

---

## 🌟 Highlights
- Designed for real-world, production environments
- Covers both **MLOps** and **modular software engineering**
- Showcases **YAML-based automation**, **logging**, and **versioning**
- Ideal template for interviews, demos, and enterprise workflows

> **"Built with the same mindset used in production teams — scalable, testable, and deployable."**

---



*Coming Soon in repo images folder...*

---

## ⭐ Give a Star
If this repo helped you understand real-world DS pipelines, consider starring it!

