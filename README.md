# Aviation Accident Data Analysis

Exploratory data analysis of a historical aviation accident dataset using Python, pandas, NumPy, and Matplotlib.

## Repository Metadata

**Suggested repository name:** `aviation-accident-data-analysis`

**Suggested GitHub description:** Exploratory Python analysis of historical aviation accident records, with data cleaning, visualizations, and trend insights.

## Project Overview

This project analyzes a historical aviation accident dataset to identify patterns in recorded accident counts, fatalities, aircraft types, operators, countries, weekdays, and yearly trends.

The analysis is contained in [`Progetto_7_Leone_Parasporo.ipynb`](Progetto_7_Leone_Parasporo.ipynb), which has been cleaned and structured for public GitHub publication.

## Questions Explored

- Which countries have the most recorded aviation accidents?
- Which weekdays appear most frequently in dated accident records?
- Which operators and aircraft types have the largest recorded fatality totals?
- How did recorded accident counts and fatalities change over time?
- Is there a relationship between annual accident counts and annual recorded fatalities?

## Dataset

The notebook loads the dataset from:

```text
https://proai-datasets.s3.eu-west-3.amazonaws.com/aviation-accidents.csv
```

The dataset includes accident records with fields such as date, aircraft type, registration, operator, fatalities, location, country, accident category, and year.

## Key Findings

- The United States has the largest number of recorded accidents in the dataset.
- Friday is the most frequent weekday among records with a complete date.
- Accident counts peak during the World War II period, especially 1944 and 1945.
- Recorded fatalities peak in 2001, showing that accident frequency and severity can move differently.
- Aircraft and operator rankings are descriptive totals from the dataset, not normalized safety rankings.

## Important Limitations

This dataset contains accident records only. It does not include exposure metrics such as total flights, passenger volume, aircraft fleet size, operating years, routes, or aircraft age.

For that reason, the results should not be interpreted as airline, country, or aircraft safety rates. They are descriptive patterns within the available accident records.

## Tools Used

- Python
- pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## How to Run

1. Clone the repository.
2. Install the required Python packages:

```bash
pip install pandas numpy matplotlib jupyter
```

3. Open the notebook:

```bash
jupyter notebook Progetto_7_Leone_Parasporo.ipynb
```

4. Run the cells from top to bottom.

The notebook will use a local `aviation-accidents.csv` file if one exists in the project folder. Otherwise, it downloads the dataset from the source URL.

## Repository Structure

```text
.
├── Progetto_7_Leone_Parasporo.ipynb
└── README.md
```

## Future Improvements

- Add normalized risk metrics using flight volume or passenger data.
- Compare accident patterns by aircraft generation or time period.
- Add interactive visualizations for country and yearly trends.
- Package the cleaning steps into reusable Python functions or scripts.

