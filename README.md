# 🎬 Sentiment Analysis on IMDB Movie Reviews

## 📌 Project Overview  
This project focuses on building a **Sentiment Analysis** model that classifies **IMDB Movie Reviews** into **Positive 😀** or **Negative 😡**.  
It leverages **Natural Language Processing (NLP)** techniques and **Deep Learning** to analyze text data.  

The project demonstrates:  
- **Text Preprocessing** (cleaning, tokenization, stopwords removal, stemming, lemmatization).  
- **Vectorization Methods** → TF-IDF and Word Embeddings.  
- **Model Training** using Logistic Regression & Neural Networks (TensorFlow/Keras).  
- **Evaluation & Visualization** (confusion matrix, classification reports).  

---

## 🎯 Objectives
- Preprocess raw IMDB reviews into clean text suitable for ML/DL models.  
- Apply **TF-IDF** and **Embeddings** for text representation.  
- Build baseline model with **Logistic Regression**.  
- Train **Deep Learning Neural Network** for classification.  
- Compare results across approaches.  

---

## 📂 Dataset
- **Source:** [IMDB 50K Movie Reviews Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)  
- **Size:** 50,000 reviews → 25k Positive, 25k Negative (balanced dataset).  
- **Features:**  
  - `review`: raw text of the review.  
  - `sentiment`: label (positive/negative).  

---

## 🔎 Project Workflow  

### **1. Data Loading & Exploration**
- Load dataset into Pandas DataFrame.  
- Check class balance (`positive` vs `negative`).  
- Analyze review length distribution.  

### **2. Text Preprocessing**
Steps applied:  
- Lowercasing.  
- Remove HTML tags, punctuation, numbers.  
- Tokenization (split into words).  
- Stopword removal.  
- Stemming & Lemmatization.  

### **3. Text Representation**
- **TF-IDF Vectorization** (n-grams).  
- **Word Embeddings** using Keras `TextVectorization` & `Embedding` layers.  

### **4. Model Building**
- Baseline: **Logistic Regression + TF-IDF**.  
- Deep Learning: **Embedding → Dense Layers (Neural Network)**.  

### **5. Evaluation**
- Accuracy, Precision, Recall, F1-score.  
- Confusion Matrix visualization.  

---

## 📊 Results Summary
| Method                     | Accuracy on Test Set |
|-----------------------------|----------------------|
| TF-IDF + Logistic Regression | ~85%               |
| Neural Network + Embeddings | ~88%               |

✅ Neural Network with Embeddings achieved the best results.  

---

## ⚙️ How to Run the Project  

### **Step 1: Clone the Repository**
```bash
git clone https://github.com/YourUsername/Sentiment-Analysis-IMDB.git
cd Sentiment-Analysis-IMDB
