# Exploratory Data Analysis (EDA) on the Titanic Dataset

Project 01 | Data Science & AI | Python, Pandas, Seaborn, Matplotlib

## Questions
1. Did women survive more than men?
2. Did ticket class matter?
3. Was age related to survival?

## What I did
- Inspected the data with `shape`, `head`, `info`, `describe`
- Found missing values and fixed each with a stated reason
  - `age`: median of the same class and sex
  - `deck`: dropped (mostly empty)
  - `embarked`, `embark_town`: most common value (only 2 rows)
- Checked duplicates and data types (duplicates kept: the dataset has no passenger ID, so identical rows may be different people)
- Compared survival with `groupby`, `agg` and `pivot_table` by sex, class, age band, port and travelling alone

## Findings
1. **Sex:** women survived at about 74% versus about 19% for men.
2. **Class:** survival fell from about 63% (1st class) to 47% (2nd) to 24% (3rd).
3. **Age:** children had the highest survival rate; see the age band table in the notebook for exact figures.

These are associations, not proof of cause.

## Run it
Open `titanic_eda.ipynb` in Jupyter or Google Colab and choose **Run all**. The data loads with `sns.load_dataset("titanic")`.
