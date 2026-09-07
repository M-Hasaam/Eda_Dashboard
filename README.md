# CSV Explorer

A Streamlit-based exploratory data analysis interface for CSV datasets.

## Features

- Validated CSV upload with a 50 MB size limit
- Dataset dimensions and first-five-row preview
- Column data types and missing-value counts
- Numerical summary with mean, median, minimum, and maximum
- Dynamic numerical/categorical attribute detection
- Histogram rendering for numerical columns
- Frequency bar chart with percentages for categorical columns

## Run locally

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
streamlit run app.py
```

Then open the local URL shown by Streamlit and upload `titanic.csv` from the sidebar. Select `Age` or `Fare` for a histogram and `Sex`, `Pclass`, or `Embarked` for a categorical frequency chart.

## Deploy

This app can be deployed to Streamlit Community Cloud by selecting this repository, setting the main file to `app.py`, and using `requirements.txt` for dependencies.
