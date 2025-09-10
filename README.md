# AI-Driven Threat Detection & Prioritization

## 📌 Project Overview
Security teams face an overwhelming number of alerts from monitoring systems, leading to "alert fatigue" and the risk of missing critical threats. This project aims to build an **AI-powered system** that intelligently detects, prioritizes, and scores threats in real-time to help cybersecurity teams respond effectively.

The system processes network data, applies machine learning algorithms, and presents actionable insights through a web interface for visualization, alert management, and tracking.

---

## 📂 Features
✅ **Real-time anomaly detection**  
✅ **Threat scoring and prioritization** based on risk levels  
✅ **Interactive dashboard** for visual insights and alert management  
✅ **Machine learning models** including Random Forest, XGBoost, and Neural Networks  
✅ **Data preprocessing pipelines** for handling imbalanced datasets  
✅ **Model explainability and reporting** using feature importance and visualization  
✅ **Secure environment setup** with `.env` configuration  
✅ **Scalable and modular architecture** for integration with other systems

---

## 🚀 Installation

### Prerequisites
- Python 3.11 or above  
- `pip` installed  
- Virtual environment tool (`venv` recommended)

### Steps

1️⃣ Clone the repository:
``bash
git clone https://github.com/0Manav0/AI-threat-detect.git

NOTE : YOU MUST HAVE TO SAVE THE MAIN(PARENT) FOLDER AS cybersecurity-threat-ai-main

2️⃣ Create and activate a virtual environment:

python -m venv venv
source venv/bin/activate    # For Linux/macOS
venv\Scripts\activate       # For Windows


3️⃣ Install the required dependencies:

pip install -r requirements.txt


4️⃣ Set up environment variables:

python -m venv venv
source venv/bin/activate    # For Linux/macOS
venv\Scripts\activate       # For Windows

5️⃣ Run the application:

python src/deploy.py


📁 Project Structure

cybersecurity-threat-ai-main/               
├── models/                # Trained ML models
├── data/(you have to unzip the folder)                  # Input datasets
├── templates/             # HTML templates
├── static/                # CSS, JS, and images
├── src                   # python files of AI(includes deploy.py,train.py,predict.py and preprocess.py)
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
├── .gitignore

#SPECIAL NOTE: PLEASE PLACE preprocessing-checkpoint.ipynb and all .ipynb FILES INSIDE A FOLDER NAMED .ipynb_checkpoints, sorry for inconvinence


📖 How it works

Data Ingestion:
Network data logs or synthetic datasets are loaded, cleaned, and preprocessed.

Feature Engineering:
Important features like traffic rate, protocol behavior, and historical patterns are calculated.

Model Training:
Algorithms like Random Forest, XGBoost, and Neural Networks are trained on labeled data.

Anomaly Detection:
Incoming data is scored based on the trained models to detect suspicious activity.

Alert Prioritization:
Alerts are ranked based on severity using a combination of statistical thresholds and model output.

Visualization:
A web dashboard displays charts, graphs, and logs to help analysts make decisions.



⚙ Usage

Run locally for testing and analysis.

Extend models with additional data or tuning parameters.

Deploy using gunicorn, Docker, or cloud platforms like AWS, GCP, or Heroku.

Integrate with other SIEM tools using APIs.









