
# 📘 Glassdoor Job Reviews – Job Recommendation System  

This repository contains the implementation of a **Job Recommendation System** based on the **Glassdoor Job Reviews dataset**.  
The study integrates **numeric features** (ratings, work-life balance, culture, etc.) and **textual features** (pros, cons, headlines, job descriptions) to predict job suitability and generate recommendations.  

---

## 📂 Dataset  

We use the **Glassdoor Job Reviews dataset** ([Kaggle link](https://www.kaggle.com/datasets/davidgauthier/glassdoor-job-reviews-2)), which contains:  
- **Textual Data**: Pros, cons, headline, job descriptions, reviews  
- **Numeric Data**: Work-life balance, compensation, culture & values, senior management, rating  
- **Targets**: Firm recommendation, CEO approval, outlook categories  

---

## 🚀 Models Implemented  

We evaluate both **baseline models** and **advanced models** for textual and numeric features.  

### 🔹 Baselines  
- LSTM  
- BiLSTM  
- BERT  
- RoBERTa  
- DistilBERT  
- HAN (Heterogeneous Attention Network)  
- GraphSAGE  

### 🔹 Proposed Model  
- Custom **Graph Neural Network (GNN)** for job recommendation  

---

## 🛠️ Features  

✔️ **Exploratory Data Analysis (EDA)** for both numeric and textual features  
✔️ **Preprocessing**: text cleaning, tokenization, scaling, graph construction  
✔️ **Model Training** with PyTorch & HuggingFace  
✔️ **Evaluation**: classification reports, confusion matrices  
✔️ **Training/Validation Curves** for loss and accuracy  
✔️ **Embedding Visualization**: t-SNE & UMAP projections  
✔️ **Graph Node Visualization** using NetworkX  
✔️ **Confidence Predictions** (model certainty for each recommendation)  
✔️ **Sample Job Recommendations**  

---

## 📊 Results  

- **Textual Feature Models**: RoBERTa achieved strong contextual understanding, while HAN and GraphSAGE showed superior graph-based representation.  
- **Numeric Feature Models**: GNN captured cross-feature dependencies better than LSTM/BiLSTM and achieved higher robustness.  
- **Proposed GNN**: Outperformed all baselines with richer embeddings, better generalization, and explainable node-level predictions.  

---

## 📈 Visualizations  

- Confusion Matrices for each model  
- Training vs Validation Accuracy/Loss curves  
- Embedding visualizations (t-SNE, UMAP)  
- Graph visualizations of job–review–firm networks  

---

## 📂 Repository Structure  

```
📦 glassdoor-job-recommendation
 ┣ 📜 README.md
 ┣ 📜 requirements.txt
 ┣ 📜 glassdoor_textual_pipeline.ipynb     # Full pipeline for textual features
 ┣ 📜 glassdoor_numeric_pipeline.ipynb     # Full pipeline for numeric features
 ┣ 📂 data/
 ┃ ┗ 📜 glassdoor_reviews.csv
 ┣ 📂 outputs/
 ┃ ┣ 📊 confusion_matrices/
 ┃ ┣ 📊 training_curves/
 ┃ ┣ 📊 embeddings/
 ┃ ┗ 📊 graph_visualizations/
```

---

## 🔧 Installation  

```bash
# Clone repo
git clone https://github.com/yourusername/glassdoor-job-recommendation.git
cd glassdoor-job-recommendation

# Install dependencies
pip install -r requirements.txt
```

---

## ▶️ Running the Notebooks  

1. Open `glassdoor_textual_pipeline.ipynb` for **textual feature training**  
2. Open `glassdoor_numeric_pipeline.ipynb` for **numeric feature training**  
3. Run all cells to reproduce results (confusion matrices, reports, recommendations).  

---
