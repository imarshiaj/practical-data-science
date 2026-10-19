# Practical Data Science: Working with Data (No Machine Learning)

A beginner-friendly, notebook-first curriculum for **collecting, cleaning, transforming, exploring, visualizing, and statistically interpreting data** with Python. The course deliberately stops before machine learning.

## What you will practice

- Practical Python used in data workflows
- NumPy arrays and pandas DataFrames
- CSV and Excel I/O, SQL with SQLite, JSON APIs, and HTML parsing
- Missing values, duplicates, types, outliers, and multi-source integration
- `groupby`, aggregation, reshaping, dates, and ranking
- Exploratory data analysis (EDA) and descriptive statistics
- Matplotlib, Seaborn, and interactive Plotly charts
- Probability, confidence intervals, bootstrap, hypothesis testing, and A/B tests
- Short, reproducible case studies with data-quality notes

## Repository structure

```text
Data Science - Working with Data/
├── 1. Practical Python Foundations/
├── 2. NumPy & Pandas/
├── 3. Data Collection/
├── 4. Data Cleaning & Preparation/
├── 5. Data Manipulation & Transformation/
├── 6. Exploratory Data Analysis/
├── 7. Data Visualization/
├── 8. Statistics for Data Analysis/
├── 9. Practical Case Studies/
├── datasets/
├── requirements.txt
└── README.md
```

## Setup

Python 3.10 or newer is recommended.

```bash
python -m venv .venv
# Windows PowerShell: .venv\Scripts\Activate.ps1
# macOS/Linux: source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
jupyter notebook
```

You can also open notebooks in JupyterLab, VS Code, or Google Colab. If you use Colab, upload the repository or open it from GitHub; the two small CSV previews are included in `datasets/`.

## Datasets and network use

- `datasets/tips_sample.csv` is a small preview of the public `tips` sample dataset in the [seaborn-data repository](https://github.com/mwaskom/seaborn-data/blob/master/tips.csv). Its source is associated with the R `reshape2` tips example; see the [repository data-source notes](https://github.com/mwaskom/seaborn-data#data-sources).
- `datasets/flights_sample.csv` contains the first four years of the `flights` example dataset (1949–1952); see [seaborn-data flights.csv](https://github.com/mwaskom/seaborn-data/blob/master/flights.csv).
- The sales-audit case study explicitly creates **synthetic** data for teaching.
- The collection notebooks use local/mock examples by default. Optional network code is commented out or behind a boolean flag. Enable it only after checking API documentation, website policies, and internet availability.

The two local public-dataset previews are intentionally small and should not be used to make population-level claims. The case-study notebooks include a `USE_FULL_DATASET` switch for loading the full public CSV from its source when online.

## Learning path

Follow the numbered folders from 1 to 9. Each notebook includes explanations, runnable examples, common caveats, and short practice prompts with suggested solutions. Run code cells in order and read the notes around each output; the chart is part of the analysis, not just decoration.

## Principles used throughout

1. Inspect raw data before changing it.
2. Keep original records when a cleaning decision may need review.
3. Make assumptions explicit, especially around missing values and outliers.
4. Use SQL parameters rather than interpolating untrusted strings into queries.
5. Respect API terms, site policies, rate limits, privacy expectations, and access controls.
6. Report both effect size and uncertainty where statistics are used.
7. Correlation and descriptive patterns do not establish causation.

## Suggested project summary for GitHub

**Practical Data Science with Python** — a notebook-based guide to data collection, cleaning, transformation, exploratory analysis, visualization, and applied statistics using NumPy, pandas, Matplotlib, Seaborn, Plotly, SQL, requests, and BeautifulSoup. No machine-learning models are covered.
