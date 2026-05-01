# 🎬 Movie Recommendation System

## 📌 Overview
This project is a **Content-Based Movie Recommendation System** that suggests movies similar to a given input using Natural Language Processing (NLP) techniques. It leverages **TF-IDF vectorization** and **cosine similarity** to compute relationships between movies based on their metadata such as overview and genres.

---

## 🎯 Motivation
With the rapid growth of digital content, users often face difficulty in finding relevant movies. This project aims to simplify content discovery by providing intelligent recommendations based on movie features, similar to modern streaming platforms.

---

## 🎯 Objective
- Convert movie metadata into numerical representations  
- Compute similarity between movies  
- Recommend top-N similar movies efficiently  
- Provide an interactive user interface  

---

## 🧠 Methodology

### 🔹 Data Preprocessing
- Load dataset (`movies_metadata.csv`)  
- Handle missing values  
- Clean and normalize text  
- Select relevant features (overview, genres)  

### 🔹 Feature Extraction (TF-IDF)
- Convert textual data into numerical vectors  
- Capture importance of words across documents  

### 🔹 Similarity Computation

Cosine Similarity Formula:

```bash
Cosine Similarity = (A · B) / (||A|| × ||B||)
```

- Measures similarity between movie vectors  
- Higher value → more similar movies  

### 🔹 Recommendation Logic
1. User inputs a movie name  
2. System finds the movie index  
3. Computes similarity scores  
4. Sorts and retrieves top-N similar movies  

---

## 🏗️ Project Structure

```bash
movie_recommendation_system/
│
├── MRS.ipynb # Model building & preprocessing
├── app.py # Streamlit web application
├── main.py # Recommendation logic
├── movies_metadata.csv # Raw dataset
│
├── df.pkl # Processed dataset
├── indices.pkl # Movie index mapping
├── tfidf.pkl # TF-IDF model
├── tfidf_matrix.pkl # Feature matrix
│
└── README.md
```
---

## ⚙️ Installation & Setup

```bash
git clone https://github.com/aashcharyakumargupta/movie_recommendation_system.git
cd movie_recommendation_system
pip install pandas numpy scikit-learn streamlit
streamlit run app.py
```
