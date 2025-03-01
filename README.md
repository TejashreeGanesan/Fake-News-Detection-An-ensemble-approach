# Fake-News-Detection-An-ensemble-approach

## 📌 Overview
This project aims to detect fake news using an **ensemble approach** that combines **LSTM (Long Short-Term Memory) networks** and **Random Forest Classifier**. The LSTM model extracts meaningful embeddings from the news text, which are then used as input to a Random Forest classifier for final classification. 🔍

## 🛠️ Technologies Used
- Python 🐍
- TensorFlow/Keras 🤖
- Scikit-Learn 📊
- Natural Language Processing (NLP) ✍️
- Random Forest Classifier 🌲
- LSTM (Long Short-Term Memory) 🔄

## 📂 Dataset
Dataset link: https://www.kaggle.com/datasets/emineyetm/fake-news-detection-datasets

The dataset consists of two CSV files:
- **Fake.csv** – Contains fake news articles ❌
- **True.csv** – Contains real news articles ✅

Each dataset includes a column `text`, which contains the news content.

## 🔄 Data Preprocessing
1. **Cleaning the text** (removing URLs, special characters, and extra spaces) ✨
2. **Labeling**
   - Fake news → `0`
   - Real news → `1`
3. **Splitting the dataset** into training (80%) and testing (20%) data 📊
4. **Tokenization & Padding** (to ensure all text inputs have the same length) 🏗️

## 🏗️ Model Architecture
### 🔹 LSTM Model
- **Embedding Layer**: Converts words into dense vector representations 📏
- **LSTM Layer**: Captures sequential dependencies in the text 🔄
- **Dropout & Regularization**: Reduces overfitting 🔥
- **Dense Layer**: Outputs a probability score for fake/real news 🎯

### 🔹 Random Forest Classifier
- LSTM embeddings are extracted and used to train a **Random Forest Classifier** to improve performance 🚀

### 🔹 Ensemble Approach
- The combination of **LSTM for feature extraction** and **Random Forest for classification** leverages both deep learning and traditional machine learning for improved accuracy and robustness ⚡📈

## 🏋️ Training & Evaluation
- **Early Stopping** is used to prevent overfitting ⏳
- **Cross-validation** is performed on the Random Forest model ✅
- **Evaluation Metrics**: Classification report & accuracy score 📊

## 📈 Results
- Achieved an accuracy of **0.97%** 🎯
- Improved model generalization using **dropout and L2 regularization** 💡
- Ensemble approach further boosts classification performance 🚀

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/TejashreeGanesan/Fake-News-Detection-An-ensemble-approach.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the script:
   ```bash
   python fake_news_detection.py
   ```



