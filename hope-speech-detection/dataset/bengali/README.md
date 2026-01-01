# 📌 BongHope: An Annotated Corpus for Bengali Hope Speech Detection  

## 📖 Table of Contents  
- [About the Project](#about-the-project)  
- [Dataset Details](#dataset-details)  
- [Features](#features)  
- [Usage](#usage)  
- [Citation](#citation)  
- [Contact](#contact)  

---

## 🔍 About the Project  
**BongHope** is a manually annotated corpus designed for **Hope Speech Detection** in Bengali social media text.  
Hope Speech refers to positive, supportive, and encouraging language that promotes harmony and resilience. This dataset enables researchers and practitioners to build models that can automatically detect hope speech, contributing to healthier online communities.  

---

## 📊 Dataset Details  
- **Source:** Collected from **Twitter (X)** and **YouTube**  
- **Format:** `.ods` (OpenDocument Spreadsheet)  
- **Size:** **4,257 text samples** in Bengali  
- **Labels:**  
  - `1` → Hope  
  - `0` → Non-hope  
- **Ground Truth Column:** `label_pred`  

📂 Dataset Repository: [BongHope Dataset](https://github.com/sayed24cse/thesis-research/tree/main/hope-speech-detection)  

---

## ✨ Features  
- ✅ First annotated corpus for **Bengali Hope Speech Detection**  
- ✅ Balanced dataset with clear binary labels  
- ✅ Useful for **text classification, NLP research, and social media analysis**  
- ✅ Supports **machine learning & deep learning experiments**  

---

## 🚀 Usage  
You can use this dataset for:  
- **Preprocessing & Tokenization** of Bengali text  
- **Training ML/DL models** (e.g., Logistic Regression, SVM, LSTM, BERT)  
- **Benchmarking Hope Speech detection tasks**  
- **Cross-lingual studies** comparing Bengali with other languages  

### Example (Python + Pandas)  
```python
import pandas as pd

# Load dataset
df = pd.read_excel("bonghope_dataset.ods")

# Preview
print(df.head())

# Separate features and labels
X = df['text']
y = df['label_pred']
