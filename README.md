# Fake News Detection Web Application

A machine learning-based web application that detects fake news articles using Natural Language Processing (NLP). Built with Flask and Scikit-learn.

## 🚀 Features
- Real-time fake news detection
- Probability confidence scores
- Clean and responsive user interface
- Visualizations of model metrics

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/ayyapparaja227-arch/Fake-News-Detector.git
   cd Fake-News-Detector
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Prepare the Model**
   > **Note:** The `tfidf_vectorizer.pkl` file is too large for GitHub. You must generate it locally before running the app.
   
   Run the training script to generate the model and vectorizer:
   ```bash
   python train_model.py
   ```

4. **Run the Application**
   ```bash
   python app.py
   ```
   Access the app at `http://127.0.0.1:5050`

## 📂 Project Structure
```
FakeNewsDetection/
├── app.py                  # Flask application entry point
├── train_model.py          # Script to train the ML model
├── requirements.txt        # Python dependencies
├── static/                 # CSS and images
├── templates/              # HTML templates
├── model/                  # Directory for saved models
│   ├── fake_news_model.pkl # Trained Classifier
│   └── metrics.pkl         # Model performance metrics
└── data/                   # Dataset directory
```

## 🤖 Model Details
- **Algorithm:** Logistic Regression / PassiveAggressiveClassifier (configurable)
- **Vectorization:** TF-IDF (Term Frequency-Inverse Document Frequency)
- **Dataset:** Contains labeled real and fake news articles.

## 👥 Author
**Ayyapparaja**
