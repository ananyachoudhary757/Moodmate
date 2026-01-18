# 🤖 MoodMate: AI Mood Predictor & Activity Recommender

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-1.28.0-red)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Model-orange)
![License](https://img.shields.io/badge/License-MIT-green)

**MoodMate** is an intelligent web application designed to analyze your emotions and provide personalized recommendations to uplift or match your mood. Built with **Python** and **Streamlit**, it leverages **Machine Learning (TF-IDF + Logistic Regression)** to detect emotions from text input and suggests curated activities, movies, music, and books.

---

## 🚀 Key Features

*   **🎙️ AI-Powered Mood Detection**: Uses Natural Language Processing (NLP) to classify text into moods like *Happy, Sad, Angry, Stressed, Tired, Calm*, and more.
*   **🧠 Hybrid Analysis Engine**: Combines a Machine Learning model (trained on 15,000+ samples) with a robust rule-based fallback system for maximum accuracy.
*   **✨ Personalized Recommendations**:
    *   **Movies**: Curated lists with posters and trailer links.
    *   **Activities**: Wellness tips, hobbies, and social suggestions.
    *   **Music & Books**: Genre and title recommendations tailored to your emotional state.
    *   **Wellness Tools**: Guided meditation and exercise suggestions.
*   **📊 History Tracking**: Automatically logs your mood entries with timestamps and confidence scores for self-reflection.

---

## 🛠️ Installation & Setup

Follow these steps to set up the project locally.

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/Moodmate.git
cd Moodmate
```

### 2. Create a Virtual Environment (Recommended)
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac/Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
Install the required Python packages using the provided `requirements.txt` file.
```bash
pip install -r requirements.txt
```

### 4. Download the Dataset
This application requires an emotion dataset to train its machine learning model.
1.  Download the **Emotions Dataset for NLP** from [Kaggle](https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp).
2.  Extract the files (`train.txt`, `val.txt`, `test.txt`) into the root directory of the project.

> **Note:** On the first run, the app will automatically download necessary NLTK corpora (stopwords, wordnet).

---

## 🖥️ Usage

Run the Streamlit application:
```bash
streamlit run app.py
```

1.  **Enter Text**: Type how you are feeling in the text box (e.g., *"I am feeling a bit overwhelmed with work today"*).
2.  **Analyze**: Click the **"Analyze Mood"** button.
3.  **View Results**: See the predicted mood, confidence score, and explore the tailored recommendations for movies, music, and activities.

---

## 📂 Project Structure

```text
Moodmate/
├── app.py                  # Main application source code
├── requirements.txt        # Python dependencies
├── posters/                # Directory for movie poster images
├── mood_history.csv        # Log of user mood entries (auto-generated)
├── mood_model.pkl          # Trained ML model (auto-generated)
├── vectorizer.pkl          # TF-IDF Vectorizer (auto-generated)
├── train.txt               # Dataset (must be added)
├── val.txt                 # Dataset (must be added)
└── test.txt                # Dataset (must be added)
```

---

## 🧠 Model Details

The core of MoodMate is a **Logistic Regression** classifier trained on a text dataset.
*   **Preprocessing**: Text cleaning, tokenization, lemmatization, and stopword removal.
*   **Vectorization**: TF-IDF (Term Frequency-Inverse Document Frequency) with n-grams (1,2).
*   **Performance**: The model achieves high accuracy on validation data and supports continuous retraining.

---

## 🤝 Contributing

Contributions are welcome! If you have suggestions for new features or better recommendation data:
1.  Fork the repository.
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

---

it is a group project. Contribuiters name mentioned below:-
1. Ananya Choudhary
2. Anuska Chatterjee
3. Ashmita Chatterjee
4. Nandini Sarkar
