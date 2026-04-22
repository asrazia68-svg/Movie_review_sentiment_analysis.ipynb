## 🎬 IMDB Sentiment Analysis & Recommendation System

---

# 📌 Project Overview

This project is a Machine Learning-based Sentiment Analysis System built on the IMDB movie reviews dataset.
It classifies user reviews into:

Positive (1)
Negative (-1)
Neutral (0)

Additionally, it provides a movie recommendation decision based on sentiment score.

---

# 🚀 Features
. Text preprocessing (cleaning, stopwords removal, lemmatization)
. TF-IDF feature extraction
. Sentiment classification using Linear SVM (LinearSVC)
. Custom recommendation system:
   . 👍 Recommend movie
   . 👎 Do not recommend
   . 🤔 Neutral suggestion
Overfitting detection (training vs testing accuracy)
# 🛠️ Technologies Used
Python
NumPy
Pandas
NLTK
Scikit-learn

--- 

# 📂 Dataset

IMDB Movie Reviews Dataset
Contains labeled reviews (positive, negative, neutral)

---

# ⚙️ Workflow

# 1. Data Loading

df = pd.read_csv('/content/IMDB Dataset.csv')

---
# 2. Sentiment Mapping

Positive → 1
Negative → -1
Neutral → 0

--- 

# 3. Text Preprocessing 

Remove HTML tags
Remove special characters
Convert to lowercase
Remove stopwords
Lemmatization

---

# 4. Feature Extraction

TF-IDF Vectorization (Top 5000 features)

--- 

# 5. Model Training

Algorithm: LinearSVC
Regularization parameter: C = 0.01

---
# 6. Evaluation

Accuracy Score
Classification Report 

---

# 7. Recommendation System

The system uses decision_function score to decide:

**Score Range** 	 **Sentiment**     **Recommendation**
> 0.1	             Positive    	        Recommend movie
< -0.1	            Negative	           Do not recommend
-0.1 to 0.1   	    Neutral             	Maybe watch
# 📊 Example Output

Score: 0.85, Sentiment: 1, Action: Recommend movie

---

# 📉 Overfitting Check

Compares training and testing accuracy
Warns if model is overfitting

---

# ▶️ How to Run

Install dependencies:
pip install numpy pandas nltk scikit-learn
Download NLTK data:
import nltk
nltk.download('stopwords')
nltk.download('wordnet')
Run the script:
python main.py

---

# 🧪 Test Your Own Review

get_recommendation("This movie was amazing!")

# 📌 Future Improvements

. Add Deep Learning models (LSTM, BERT)
. Improve neutral sentiment detection
. Deploy as a web app (Flask/Streamlit)

---

# ⭐ Conclusion

This project demonstrates how Natural Language Processing (NLP) and Machine Learning can be used to analyze user opinions and provide intelligent recommendations.
