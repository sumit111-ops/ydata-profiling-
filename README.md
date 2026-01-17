# ydata-profiling-
ydata profiling on jupyter notebook as my first repo


📊 Netflix Exploratory Data Analysis (EDA)
📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on the Netflix Movies and TV Shows dataset using Python, Pandas, and YData Profiling.
The goal is to understand the dataset structure, identify missing values, analyze distributions, and extract meaningful insights before any machine learning modeling.

📂 Dataset

Name: Netflix Movies and TV Shows

Source: Kaggle

Format: CSV

Rows: ~8,800

Columns: Movies/TV metadata such as type, title, country, rating, duration, release year, etc.

🛠️ Tools & Libraries Used

Python

Pandas

Matplotlib & Seaborn (for manual EDA)

YData Profiling (automated EDA report)

🚀 Project Workflow

Data Loading & Basic Inspection

Handling Encoding Issues

Automated EDA using YData Profiling

Manual EDA for deeper insights

Interpretation of patterns and trends

⚙️ Installation & Setup
Recommended Environment

Python 3.10

Install Required Libraries
pip install pandas matplotlib seaborn ydata-profiling

▶️ How to Run the Project
1️⃣ Load the dataset
import pandas as pd

df = pd.read_csv("netflix_titles.csv", encoding="latin1")

2️⃣ Generate YData Profiling Report
from ydata_profiling import ProfileReport

profile = ProfileReport(
    df,
    title="Netflix EDA Report",
    explorative=True
)

profile.to_file("output.html")

3️⃣ Open the Report

Open output.html in your browser to view the full interactive EDA report 

output

.

📈 Key Insights

Netflix hosts more Movies than TV Shows

Majority of content was released after 2010

USA contributes the highest number of titles

Significant missing values in director, cast, and country

TV Shows are generally more recent than Movies

⚠️ Limitations

Automated profiling may be slow for very large datasets

Domain-specific insights still require manual EDA

Profiling should not replace feature engineering

🎯 Use Cases

Beginner to Intermediate EDA practice

Resume & GitHub portfolio project

Interview discussion (EDA + data quality)

Preprocessing step before ML modeling

📌 Interview Talking Point

“I used YData Profiling to quickly understand data quality and distributions, followed by manual EDA for deeper insights and feature engineering decisions.”

📁 Project Structure
├── netflix_titles.csv
├── output.html
├── eda_notebook.ipynb
└── README.md

🔮 Future Improvements

Feature engineering for recommendation systems

Sentiment analysis on descriptions

ML model for content popularity prediction

👤 Author

Sumit
Aspiring Data Scientist / ML Enginee
