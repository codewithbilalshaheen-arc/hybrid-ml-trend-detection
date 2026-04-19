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
