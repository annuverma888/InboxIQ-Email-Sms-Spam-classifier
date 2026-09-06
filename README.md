# InboxIQ: Intelligent Email Classification & Spam Detection

InboxIQ is a machine learning-powered text classification application designed to accurately identify and filter out spam or unwanted email messages. Built with Python, scikit-learn, and Natural Language Processing (NLTK), it boasts high accuracy and precision, making it an ideal engine for a production-ready email inbox assistant.

## 🚀 Live Demo

[![Open InboxIQ](https://img.shields.io/badge/🎬%20Open-InboxIQ-red?style=for-the-badge)](https://inboxiq-email-sms-spam-classifier.streamlit.app/)

## 🚀 Features
- **Exploratory Data Analysis (EDA):** Deep analysis of dataset class distributions, character lengths, word counts, and sentence counts using visualization tools like seaborn and matplotlib.
- **Advanced Text Preprocessing:** Includes custom pipeline steps for lowercasing, word tokenization, punctuation removal, stopword removal, alphanumeric filtering, and Porter Stemming.
- **Term Frequency-Inverse Document Frequency (TF-IDF):** Text vectorization optimized up to 3000 top features for superior model training.
- **Multiple Model Evaluation:** Comparative execution and baseline results for Naive Bayes variants (Gaussian, Multinomial, Bernoulli), Support Vector Machines, Random Forest, Stacking, and Voting Ensembles.
- **Optimized for High Precision:** Selected Naive Bayes and Ensemble configurations achieving exceptional performance and near-flawless precision scores to avoid false positives.

## 🛠️ Project Structure
```text
├── inboxiq.ipynb        # Comprehensive Jupyter notebook with full model analysis
├── app.py               # Streamlit web application frontend (if applicable)
├── model.pkl            # Pickled, fully-trained classification model
├── vectorizer.pkl       # Pickled TF-IDF vectorizer configuration
├── requirements.txt     # Complete list of installation dependencies
└── README.md            # Project documentation and onboarding instructions
```

## 📊 Model Performance Baseline
Based on our experimental analysis of structural modifications, feature engineering, and model variations, the evaluation profile highlights:

| Algorithm | Accuracy | Precision |
| :--- | :--- | :--- |
| **Multinomial Naive Bayes (MNB)** | 97.10% | **100%** |
| **K-Nearest Neighbors (KNN)** | 90.52% | **100%** |
| **Random Forest (RF)** | 97.49% | 98.28% |
| **Extra Trees Classifier (ETC)** | 97.78% | 97.52% |
| **Support Vector Classifier (SVC)** | 97.58% | 97.48% |
| **Logistic Regression (LR)** | 95.55% | 96.00% |

*Note: Multinomial Naive Bayes (MNB) coupled with TF-IDF Vectorization serves as our champion model owing to its flawless precision score, mitigating the risk of misclassifying crucial user emails as spam.*

## ⚙️ Installation & Onboarding

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/inboxiq.git
cd inboxiq
```

### 2. Set Up a Virtual Environment
```bash
# Windows
python -m venv inboxiq
inboxiq\Scripts\activate

# macOS/Linux
python3 -m venv inboxiq
source inboxiq/bin/activate
```

### 3. Install Required Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run Application
```
streamlit run app.py
```

## 🧠 Technologies Used
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, NLTK, XGBoost, Matplotlib, Seaborn, WordCloud


