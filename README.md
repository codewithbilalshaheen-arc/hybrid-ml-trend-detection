<<<<<<< HEAD
=======
# Hybrid ML System for Detecting Emerging Digital Trends

## Project Description
This project uses LDA (Latent Dirichlet Allocation) topic modeling combined with change point detection to automatically identify emerging trends from Reddit comments.

## Team Roles

### Saqib Hayat - Data Engineer
- Data collection, cleaning & preprocessing
- Time series data preparation

### Shehbaz Makhmoor Ali - ML Engineer
- LDA model development
- Topic assignment and visualization
- Interactive charts

### Muhammad Bilal - Analytics Engineer
- Change point detection
- Dashboard development
- Final report and presentation

## Tech Stack
- Python, Pandas, NumPy
- Scikit-learn, Gensim (LDA)
- Ruptures (Change Point Detection)
- Streamlit (Dashboard)
- Plotly (Visualizations)

## Folder Structure

```
hybrid-ml-trend-detection/
│
├── data/                          # Dataset storage
│   ├── raw/                       # Original downloaded datasets
│   ├── clean_reddit_data.csv      # Preprocessed dataset (Week 1)
│   └── topic_time_series.csv      # Topic counts by week (Week 2)
│
├── notebooks/                                   # Jupyter notebooks for analysis
│   ├── 1_data_preprocessing_and_lda.ipynb       # Week 1: Data cleaning + LDA
│   ├── 2_time_series_creation.ipynb             # Week 2: Time series generation
│   └── 3_change_point_detection.ipynb           # Week 2: Trend detection
│
├── src/                           # Python source code modules
│   ├── preprocessing.py           # Data cleaning functions
│   ├── lda_model.py               # LDA training and evaluation
│   ├── change_detection.py        # Change point detection logic
│   └── utils.py                   # Helper functions
│
├── outputs/                          # Generated results and visualizations
│   ├── word_clouds/                  # Topic word clouds (PNG files)
│   ├── plots/                        # Time series and change point plots
│   ├── lda_model.pkl                 # Trained LDA model
│   ├── topic_labels.csv              # Topic IDs with human-readable labels
│   ├── emerging_trends_results.csv   # Final detection results
│   └── coherence_comparison_report.pdf  # Model evaluation report
│
├── app/
│   ├── app.py                    # Main dashboard application
│   ├── components/               # Reusable UI components
│   └── assets/                   # Images, CSS for dashboard
│
├── .gitignore                    # Files to exclude from Git
├── README.md                     # Project documentation (this file)
└── requirements.txt              # Python dependencies
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/<your-team>/hybrid-ml-trend-detection.git
cd hybrid-ml-trend-detection
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Download the dataset

Download a Reddit comments dataset from Kaggle (search for *"Reddit comments 2025"* or *"World News Reddit dataset"*). Place the raw file inside `data/raw/`.

### 4. Run the notebooks in order

```bash
# Start Jupyter
jupyter notebook

# Run in this sequence:
# 1. notebooks/1_data_preprocessing_and_lda.ipynb
# 2. notebooks/2_time_series_creation.ipynb
# 3. notebooks/3_change_point_detection.ipynb
```

### 5. Launch the dashboard

```bash
streamlit run app/app.py
```

---

## Pipeline Summary

```
Raw Reddit Data
     │
     ▼
[Preprocessing]  →  clean_reddit_data.csv
     │
     ▼
[LDA Topic Model]  →  lda_model.pkl · topic_labels.csv · word clouds
     │
     ▼
[Time Series Construction]  →  topic_time_series.csv · Plotly charts
     │
     ▼
[Change Point Detection]  →  emerging_trends_results.csv · change point plots
     │
     ▼
[Streamlit Dashboard]  →  Interactive visualisations & trend explorer
```

---

## Key Outputs

| File | Description |
|------|-------------|
| `clean_reddit_data.csv`       | Preprocessed Reddit comments with timestamps |
| `lda_model.pkl`               | Serialised trained LDA model |
| `topic_labels.csv`            | Topic IDs mapped to human-readable labels and top words |
| `topic_time_series.csv`       | Weekly post counts per topic (wide format) |
| `emerging_trends_results.csv` | Topics flagged as Emerging / Stable / Declining with growth rates |

---

## Weekly Milestones

| Week | Goal | Milestone |
|------|------|-----------|
| Week 1 | Data + Preprocessing + LDA | 10–15 meaningful topics visible |
| Week 2 | Time Series + Change Point Detection | System automatically flags emerging trends |
| Week 3 | Dashboard + Report + Submission | Project fully ready for submission and viva |

---

## Team Conventions

- **Commit daily** — push to GitHub every day, even partial progress
- **Branch naming** — `feature/student-a-preprocessing`, `feature/student-b-lda`, etc.
- **Small data first** — develop and test on 5,000 rows; run the full dataset only when code works
- **Daily check-in** — share: what I did, what's next, any blockers
- **Google Colab** — use for heavy LDA training (free GPU); mount Google Drive to persist files

---

## Learning Resources

### Python & Data

| Topic | Resource |
|-------|----------|
| Python | docs.python.org/3/tutorial |
| Pandas | kaggle.com/learn/pandas |
| NumPy | numpy.org/doc/stable/user/quickstart.html |
| Google Colab | colab.research.google.com |

### NLP & LDA

| Topic | Resource |
|-------|----------|
| Tokenization / Stopwords | nltk.org/book/ch01.html |
| LDA intuition | YouTube: "Topic Modeling LDA" by StatQuest |
| Gensim LDA | radimrehurek.com/gensim |
| pyLDAvis | github.com/bmabey/pyldavis |

### Time Series & Change Point Detection

| Topic | Resource |
|-------|----------|
| Time series basics | kaggle.com/learn/time-series |
| ruptures library | centre-borelli.fr/ruptures-docs |
| Streamlit | docs.streamlit.io/get-started |

---

## License

This project was developed as part of an academic course assignment. All data used is publicly available via Kaggle.
>>>>>>> d946a920623ecd8dfef024183f4ec0d51e8e658d
