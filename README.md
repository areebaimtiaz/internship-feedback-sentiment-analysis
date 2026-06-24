# Internship Feedback Sentiment Analysis

## 📌 Objective
Evaluate the emotional tone of feedback (collected from surveys, comments, and social media) to help enhance the internship experience, using Natural Language Processing.

## 📊 Dataset
- **Source:** [Customer Feedback Dataset – Kaggle](https://www.kaggle.com/datasets/vishweshsalodkar/customer-feedback-dataset)
- Used as a proxy for intern feedback (text feedback collected from social media, review platforms, and testimonials)
- **96 rows** of feedback text

## 🛠️ Tools & Libraries
- Python
- NLTK (VADER SentimentIntensityAnalyzer)
- Pandas
- Matplotlib / Seaborn

## ⚙️ Methodology
1. Collected and cleaned feedback text data
2. Applied NLTK's VADER sentiment analyzer to compute a compound sentiment score for each entry
3. Classified each entry into **Positive**, **Neutral**, or **Negative** based on standard VADER thresholds:
   - `compound >= 0.05` → Positive
   - `compound <= -0.05` → Negative
   - otherwise → Neutral
4. Visualized the sentiment distribution with a pie chart and bar chart

## 📈 Results

| Sentiment | Percentage |
|-----------|-----------|
| Positive  | 57.3% |
| Neutral   | 1.0%  |
| Negative  | 41.7% |

**Key insight:** The majority of feedback (57.3%) is positive, suggesting overall satisfaction with the internship experience, though a notable 41.7% negative share highlights specific areas that may need improvement.

## 📁 Repository Contents
- `internship_feedback_sentiment_analysis.ipynb` — full analysis notebook
- `internship_feedback_sentiment_results.csv` — labeled output dataset
- `sentiment_pie_chart.png` — sentiment distribution (pie chart)
- `sentiment_bar_chart.png` — sentiment distribution (bar chart)

## 🚀 How to Run
1. Open the notebook in Google Colab
2. Run all cells (auto-downloads the dataset via `kagglehub`)
3. View results in the generated CSV and charts

## 👤 Author
Areeba Imtiaz — Data Analyst | BI & Python Enthusiast
