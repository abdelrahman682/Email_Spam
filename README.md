A simple yet powerful Streamlit web app to classify emails as Spam or Not Spam, using a trained LinearSVC model and TF-IDF text vectorization.

🚀 Features
🔎 Classify raw email content instantly

⚙️ Preprocessing includes lowercasing, number replacement, stopword removal, and stemming

💻 Built with Streamlit for an intuitive web UI

🔬 Model trained using scikit-learn’s LinearSVC

🧠 Tech Stack
Python 3.10+

scikit-learn for ML model

nltk for text preprocessing

joblib for model persistence

streamlit for UI

📂 Project Structure
bash
Copy
Edit
spam_detector/
├── app.py                 # Streamlit web app
├── utils.py               # Custom preprocessing functions
├── spam_model.pkl         # Trained LinearSVC model
├── tfidf_vectorizer.pkl   # Fitted TF-IDF vectorizer
└── README.md              # This file
⚙️ How to Run the App
Clone the repo or copy the files

Install dependencies:

bash
Copy
Edit
pip install streamlit scikit-learn nltk joblib
Run the app:

bash
Copy
Edit
streamlit run app.py
Open in browser:
Visit http://localhost:8501

🧹 Preprocessing Steps
Emails go through the following cleaning:

Convert to lowercase

Remove punctuation and special characters

Replace numbers with "num"

Remove common stopwords

Apply stemming (via PorterStemmer)

✅ Example
text
Copy
Edit
Original:
"Subject: WIN MONEY NOW!!! Call 123456."

After preprocessing:
"win money num call"
✨ Future Improvements
Upload email files (.txt, .csv)

Batch prediction for multiple emails

Deploy to Streamlit Cloud or Hugging Face Spaces

Improve model with deep learning (optional)

🧑‍💻 Author
Abdelrahman Soliman
Built with 💡, Python, and a lot of debugging.
