# Netflix Content Analysis - Auspify Data Science Internship (Tasks 1 to 6)

End-to-end data science project on the Netflix titles dataset (8,790 rows, 10 columns), done as one Google Colab notebook for the **Auspify Technologies** Data Science Internship. All 6 tasks are completed (the program needs any 4).

**Live dashboard:** https://akshatkesharwani-info.github.io/auspify-netflix-data-science/netflix_dashboard.html

## What is inside

| Task | Level | What was done | Key result |
|---|---|---|---|
| 1 | Easy | Data cleaning and preprocessing | Missing values hidden as "Not Given" fixed, 3 duplicates removed, 8,787 clean rows, 22 columns, 0 nulls |
| 2 | Easy | Exploratory data analysis | 12+ charts - 69.7% Movies, US leads with 3,240 titles, 45.6% adult content, only 10.3% kids content |
| 3 | Medium | Recommendation system (TF-IDF + cosine similarity) | 96.5% of recommendations share a genre vs 24.4% for random picks |
| 4 | Medium | Trend prediction (5 forecasting models) | Yearly releases peaked in 2018 and are flat since - "repeat last year" model was best (MAPE 6.0%) |
| 5 | Advanced | Movie vs TV Show classification (4 models) | Logistic Regression 94.8% accuracy vs 69.7% baseline, 5-fold CV 94.6% |
| 6 | Advanced | Business insights dashboard (Plotly) | Interactive charts, saved HTML dashboard, 7 business recommendations |

## Main findings

- The catalog is movie heavy (69.7%), US dominated (about 37%) and adult focused (45.6% adult vs 10.3% kids).
- 67.2% of TV shows have only 1 season.
- Titles released per year grew from 37 (2000) to 1,144 (2018), then fell to 953 in 2020. Trend-line models (Linear, Polynomial) kept predicting growth and were off by 23 to 30% on the test years, while the naive model was off by 6%.
- `duration` and genre columns were removed from the classifier on purpose because they give the answer away (data leakage). `has_director` ended up the strongest feature (about 68% importance) because most TV shows have no director listed.

## Files

| File | Description |
|---|---|
| `Auspify_DS_Netflix_Tasks_1-6.ipynb` | Main notebook with all 6 tasks and saved outputs |
| `Dataset.csv` | Raw Netflix dataset |
| `netflix_clean.csv` | Cleaned dataset made in Task 1 |
| `netflix_dashboard.html` | Interactive dashboard made in Task 6 (open in browser) |

## How to run

1. Open `Auspify_DS_Netflix_Tasks_1-6.ipynb` in Google Colab.
2. Run all cells (Runtime - Run all). When the first code cell asks, upload `Dataset.csv`.
3. No installs needed, Colab already has all the libraries.

GitHub does not show the interactive Plotly charts inside the notebook preview, so use the live dashboard link above or open the notebook in Colab.

## Tools used

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels, Plotly, Google Colab

## About

**Akshat Kesharwani** - Data Analyst and Data Scientist (Fresher)
Portfolio: https://akshatkesharwani-info.github.io/
GitHub: https://github.com/akshatkesharwani-info

#Auspify #AuspifyTechnologies #AuspifyInternship #AuspifyProjects
