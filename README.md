# 🛡️ Email Spam Detection System

An interactive **AI-powered email classification system** that detects whether an email is **Spam** or **Legitimate** using machine learning models.  
Built using **Python**, **NLTK**, and **Scikit-learn**, with an elegant **Voilá + ipywidgets UI** for live interaction.

---

## 🚀 Features

- 📂 **Automatic Data Loading & Cleaning**
  - Loads `spam_ham_dataset.csv`  
  - Cleans and preprocesses email text (lowercasing, punctuation removal, stemming, stopword removal)

- 🧠 **Machine Learning Models**
  - Trains and compares **Naive Bayes** and **SVM** models  
  - Displays performance results and accuracy visualization  
  - Automatically selects the best-performing model

- 💬 **Interactive Email Analysis**
  - Enter or paste your own email text  
  - Choose from preloaded **sample emails** (legit, promotional, or suspicious)  
  - One-click spam detection with confidence score and model details

- 🎨 **Beautiful Interface**
  - Modern, styled dashboard built with **ipywidgets** and **HTML**  
  - Includes header, performance cards, interactive widgets, and footer  
  - Works seamlessly in **Jupyter Notebook** or **Voilá app**

---

## 🧩 Technologies Used

| Component | Purpose |
|------------|----------|
| **Python** | Core language |
| **NLTK** | Text preprocessing, stemming, stopwords |
| **Scikit-learn** | Model training, feature extraction, evaluation |
| **Pandas / NumPy** | Data manipulation |
| **ipywidgets** | UI interactivity |
| **Voilá** | Converts notebook into a web app |

---

## 📘 Dataset

The system uses the **`spam_ham_dataset.csv`** file, which must contain at least:
- `text` — The email content  
- `label` — Either `spam` or `ham`

If the dataset includes other columns (like `Unnamed: 0`, `label_num`), they are automatically handled and removed.

---

## ⚙️ How It Works

1. **Data Preparation**
   - Cleans and preprocesses email text.
   - Converts text into numerical features using `CountVectorizer`.

2. **Model Training**
   - Trains both **Multinomial Naive Bayes** and **Support Vector Machine (SVM)** models.
   - Evaluates and selects the best-performing model based on accuracy.

3. **Prediction**
   - Cleans and vectorizes user-input email.
   - Predicts whether the email is **Spam** or **Legitimate**.
   - Displays confidence score (if available).

4. **Visualization**
   - Interactive UI for entering emails or selecting sample ones.
   - Real-time classification display.

---

## 🧠 Example Models & Performance

| Model | Description | Accuracy |
|--------|--------------|-----------|
| **Naive Bayes** | Probabilistic model suited for text classification | ~97–99
