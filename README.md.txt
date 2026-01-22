# 🔠 Roman-to-Urdu Transliteration Engine

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![NLP](https://img.shields.io/badge/NLP-Text_Processing-green)
![Status](https://img.shields.io/badge/Status-Prototype-orange)

## 📖 Project Overview
This project addresses a critical challenge in **Natural Language Processing (NLP)** for South Asian languages: **Text Normalization**.

It implements a transliteration pipeline that converts **Roman Urdu** (informal text typed in English characters) into **Formal Urdu** (Perso-Arabic script). This bridges the gap between user-generated content and standard AI models.

**Example:**
* **Input:** *tum kahan ho*
* **Output:** *تم کہاں ہو*

---

## 🏢 The Industry Problem
Most modern NLP models (like BERT-Urdu) fail on "Roman" text, yet 90% of chat/social media data in Pakistan is written in Roman characters. 

**This project solves that by acting as a Pre-Processing Layer:**
1.  **Chatbots:** Allows banking bots to understand "mera balance batado".
2.  **Search:** Enables users to type in English but find results in Urdu.
3.  **Sentiment Analysis:** Normalizes raw social media comments for accurate analytics.

---

## ⚙️ Technical Architecture

### 1. Data Processing
* **Corpus Ingestion:** Loads parallel datasets of Roman and Urdu text.
* **Tokenization:** Breaks down sentences into processable tokens.
* **Mapping Logic:** Utilizes a dictionary-based and context-aware mapping approach to handle phonetic variations (e.g., mapping both 'k' and 'q' to 'ک' or 'ق' based on context).

### 2. The Pipeline
The system reads the input file, processes the string characters against the vocabulary, and outputs the normalized Urdu script.

---

## 💻 How to Use

1.  **Clone the Repo:**
    ```bash
    git clone [https://github.com/your-username/roman-urdu-transliteration.git](https://github.com/your-username/roman-urdu-transliteration.git)
    ```

2.  **Install Dependencies:**
    ```bash
    pip install pandas numpy
    ```

3.  **Run the Notebook:**
    Open `NLPASSIGNMENT2.ipynb` to see the logic and results.

---

## 📊 Results
The system successfully handles common conversational phrases, demonstrating the ability to normalize text for downstream NLP tasks.

---

## 📜 License
This project is open-source.