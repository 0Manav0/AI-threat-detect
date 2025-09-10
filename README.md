**TEAM MEMBERS:**  
Garach Viraj  
Vaghasiya Jil  
Dedakiya Manav



*This project uses the publicly available AI model, which is licensed under the MIT License (see https://github.com/mahaswetaroy1/cybersecurity-threat-ai.git). The model was pre-trained and integrated into this project. All other components, features, and implementation were developed during the hackathon.*


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

## Step-by-Step Usage

### A. Preprocess the Data
Converts ARFF to CSV, applies label encoding.
```cmd
python src\preprocess.py
```

### B. Train the Model
Trains a Random Forest classifier on the preprocessed data.
```cmd
python src\train.py
```

### C. Test the Model Locally (Optional)
```cmd
python src\predict.py
```

### D. Deploy the API
Runs the Flask server for real-time predictions.
```cmd
python src\deploy.py
```

after that visit http://127.0.0.1:5000 and pick your request as in form and submit


📁 Project Structure

cybersecurity-threat-ai-main/

├── models/                # Trained ML models

├── data/(you must have to unzip the folder)                  # Input datasets

├── templates/             # HTML templates

├── static/                # CSS, JS, and images

├── src                   # python files of AI(includes deploy.py,train.py,predict.py and preprocess.py)

├── requirements.txt       # Python dependencies

├── README.md              # Project documentation

├── .gitignore

#SPECIAL NOTE: PLEASE PLACE preprocessing-checkpoint.ipynb and all .ipynb FILES INSIDE A FOLDER NAMED .ipynb_checkpoints also unzip data folder and check for dupicatiion in data folder, sorry for inconvinence


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









