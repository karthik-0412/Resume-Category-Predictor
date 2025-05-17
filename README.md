# Resume-Screening-App


---


# 📝 Resume Category Prediction App

A simple Streamlit-based web app that predicts the **category of a resume** (e.g., Data Science, HR, etc.) using a **machine learning model** trained on resume data. Upload resumes in PDF, DOCX, or TXT format and instantly get predictions.


## 🚀 Features

- 📂 Upload resumes in **PDF**, **DOCX**, or **TXT**
- 🧹 Automatic text extraction and preprocessing
- 🧠 ML model (SVC) with **TF-IDF** for category prediction
- 🎯 Real-time prediction with **cleaned resume text**
- 🔍 Optional: View extracted resume text before prediction

---

## 🛠️ Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/Resume-Screening-App.git
cd Resume-Screening-App
````

2. Install dependencies:

```bash
pip install -r requirements.txt
```

> Or manually:

```bash
pip install streamlit scikit-learn python-docx PyPDF2
```

3. Make sure the following files are present:

* `clf.pkl` – trained SVC model
* `tfidf.pkl` – TF-IDF vectorizer
* `encoder.pkl` – Label encoder

---

## 📦 Usage

Run the Streamlit app:

```bash
python -m streamlit run app.py
```

Then open the link shown in your terminal (usually `http://localhost:8501`) in your browser.

---

## 🧠 Model Info

* Model: `Support Vector Classifier` (SVC)
* Preprocessing: `TF-IDF` Vectorization
* Categories: Trained on various job functions from resume data

> Note: Ensure that the pickle files (`clf.pkl`, `tfidf.pkl`, `encoder.pkl`) are compatible with your `scikit-learn` version.

---

## 📁 Project Structure

```
Resume-Screening-App/
│
├── app.py                # Streamlit app source code
├── clf.pkl               # Trained SVC model
├── tfidf.pkl             # TF-IDF vectorizer
├── encoder.pkl           # Label encoder
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

---

## 🧪 Sample Files

You can test the app using sample resumes (PDF/DOCX/TXT). Just upload and get instant category predictions.

---

## ⚠️ Notes

* **InconsistentVersionWarning** may appear if your `scikit-learn` version doesn't match the one used during training. It's generally safe unless you encounter errors.
* Supports only **English resumes** currently.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🤝 Contributing

Feel free to fork, improve, and submit pull requests!

---

.

Here’s a simple `requirements.txt` for your project:

```
streamlit
scikit-learn
python-docx
PyPDF2
```

---

You can create this file by saving the above lines into a file named `requirements.txt` in your project root folder.

Then your users can install all dependencies at once with:

```bash
pip install -r requirements.txt
```

If you want, I can help generate a complete zipped project structure with the README and requirements file ready! Just let me know.

