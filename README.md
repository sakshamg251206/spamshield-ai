🧠 AI Email Spam Detection System

An end-to-end machine learning application that classifies emails into Spam or Legitimate (Ham) categories. This project focuses on building a scalable pipeline for both training and real-time inference, along with an interactive web interface for testing predictions.

🚀 What this project does
📩 Classifies email text into spam or non-spam using ML models
⚙️ Uses a modular pipeline for preprocessing, training, and prediction
🌐 Provides a simple web interface for real-time predictions
📂 Supports bulk email classification via .mbox files
📊 Tracks performance using key evaluation metrics

🛠️ Tech Stack
Python (3.10+)
Machine Learning: Scikit-learn
Frontend/UI: Streamlit
Data Handling: Pandas, NumPy
Text Processing: BeautifulSoup

📁 Project Layout
project/
│
├── app.py                # Streamlit UI
├── main.py               # Optional entry point
├── requirements.txt
│
├── src/
│   ├── pipeline/         # Training & prediction flow
│   ├── components/       # Data processing modules
│   ├── config/           # Configurations
│   └── utils/            # Helper functions
│
├── data/                 # Input datasets
├── outputs/              # Saved models & artifacts
├── logs/                 # Runtime logs


⚡ Setup Instructions
1. Clone the repo
git clone <your-repo-link>
cd your-project
2. Create virtual environment
python3 -m venv .venv
source .venv/bin/activate
3. Install dependencies
pip install -r requirements.txt
🖥️ Run the App
streamlit run app.py

You’ll get:

🔹 Single email prediction
🔹 Batch processing (upload .mbox)
🧪 Model Training (Optional)

To retrain the model:

python -m src.pipeline.training_pipeline

Make sure your dataset is placed correctly inside:

data/dataset/
📊 Evaluation

The system evaluates models using:

Accuracy
Precision
Recall
F1 Score

Best-performing model is automatically selected for predictions.