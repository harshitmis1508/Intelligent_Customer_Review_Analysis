# Intelligent_Customer_Review_Analysis
AI-based system for analyzing and predicting customer sentiment from feedback using NLP and Transformer models.
# Intelligent Customer Feedback Analysis System

**Short description**  
AI-based system that analyzes customer feedback using NLP and Transformer models (DistilBERT). Includes data cleaning, sentiment classification, summarization, visualization, and a demo app.

---

## Project structure (important files)
- `Part1_Data_Preprocessing.ipynb` — data cleaning & preprocessing, saved `clean_feedback.csv`  
- `Part2_Sentiment_Classification.ipynb` — model training (DistilBERT) and evaluation  
- `Part3_Text_Summarization.ipynb` — transformer-based summarization (T5) examples  
- `Part4_AI_Insights.ipynb` — (optional) topic extraction & forecasting — **skipped** / placeholder (see note)  
- `Part5_App_Deployment.ipynb` / `app.py` — Streamlit demo app for upload, analysis, visualization  
- `clean_feedback.csv` — cleaned dataset (used by notebooks)  
- `sentiment_model/` — saved HuggingFace model directory (or instructions to load)  
- `predicted_feedback.csv` — sample inference output  
- `AI_insights_report.pdf` — insights report (if produced)  
- `requirements.txt` — Python packages to install

---

## How to run (quick)
### 1) Run notebooks (Google Colab recommended)
Open each `Part*.ipynb` in Colab or Jupyter and run the cells in order. Important order:
1. `Part1_Data_Preprocessing.ipynb` — create `clean_feedback.csv`  
2. `Part2_Sentiment_Classification.ipynb` — trains and saves model to `sentiment_model/`  
3. `Part3_Text_Summarization.ipynb` — summarization examples  
4. `Part5_App_Deployment.ipynb` — demo / deployment instructions

### 2) Run Streamlit demo (local)
```bash
pip install -r requirements.txt
streamlit run app.py
