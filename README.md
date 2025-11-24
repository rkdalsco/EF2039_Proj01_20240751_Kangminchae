# EF2039 Project 01 – Sentiment Analysis Application  
Repository: [https://github.com/rkdalsco/EF2039_Proj01_20240751_Kangminchae](https://github.com/rkdalsco/EF2039_Proj01_20240751_Kangminchae)

## 1. Overview  
This project implements a complete AI application pipeline that analyzes user comments on a skincare product and classifies them into **Positive**, **Neutral**, or **Negative** sentiments. The objective is to learn the end-to-end development cycle: idea generation, pipeline design, model selection, environment setup, model analysis, application deployment, code management, and advertisement.

## 2. Features  
- Korean text preprocessing and cleaning  
- Keyword extraction via `KoNLPy` (Okt)  
- Sentiment classification using a pretrained model: `alsgyu/sentiment-analysis-fine-tuned-model`  
- Visualization of sentiment distribution with charts  
- Comparative evaluation using Mean Absolute Error (MAE) between initial expectations and model results

## 3. Pipeline Workflow  
1. Load raw comment data from an Excel file.  
2. Standardize and optionally summarize comments.  
3. Extract important morphemes (keywords) excluding stopwords.  
4. Run sentiment inference for each comment.  
5. Aggregate and compute sentiment distribution percentages.  
6. Visualize results and compare with baseline expectation.  
7. Document code, publish to GitHub, and prepare presentation.

## 4. Prerequisites  
- Python 3.7+  
- Libraries listed in `requirements.txt` (see below)  
- GPU optional but helpful for faster inference

## 5. Installation & Usage  
```bash
# Install dependencies
pip install -r requirements.txt

# Option A: Run the script directly
python src/sentiment_analysis.py
python src/visualization.py

# Option B: Open the Jupyter/Colab notebook
# AI_Sentiment_Project.ipynb
