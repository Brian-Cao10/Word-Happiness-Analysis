# World Happiness Analysis

This repository contains a Jupyter Notebook analysis of the World Happiness Report data from 2015 through 2019. The project combines multiple yearly datasets, standardizes their columns, explores the factors associated with happiness, and evaluates regression-based predictive approaches.

## Project Overview

The analysis focuses on understanding which variables most strongly relate to a country's happiness score, including:

- GDP per capita
- Social support / family support
- Health and life expectancy
- Freedom
- Trust / corruption perception
- Generosity

The notebook also compares rankings across years and cleans the data to build a unified dataset for analysis.

## Repository Structure

```text
Word-Happiness-Analysis/
├── World_Happiness.ipynb
├── world_happiness/
│   ├── 2015.csv
│   ├── 2016.csv
│   ├── 2017.csv
│   ├── 2018.csv
│   └── 2019.csv
└── README.md
```

## Contents

- `World_Happiness.ipynb`: Main analysis notebook containing data loading, cleaning, exploratory analysis, and model evaluation.
- `world_happiness/*.csv`: Country-level happiness datasets for each year, used as the source data for the notebook.

## Technologies Used

- Python
- pandas
- NumPy
- matplotlib
- seaborn
- scikit-learn
- SciPy
- Jupyter Notebook

## Setup

1. Clone the repository:

```bash
git clone https://github.com/Brian-Cao10/Word-Happiness-Analysis.git
cd Word-Happiness-Analysis
```

2. Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate
```

On Windows:

```bash
.venv\Scripts\activate
```

3. Install dependencies:

```bash
pip install jupyter pandas numpy matplotlib seaborn scipy scikit-learn
```

## Running the Analysis

Open the notebook in Jupyter:

```bash
jupyter notebook World_Happiness.ipynb
```

Then run the cells in order to:

- Load the yearly data files
- Standardize column names across 2015-2019
- Inspect nulls and data quality
- Review summary statistics
- Compare happiness factors across countries
- Build and evaluate regression models

## Key Analysis Tasks

The notebook includes:

- Combining five year-specific World Happiness datasets into one master dataset
- Handling inconsistent field names between years
- Exploring relationships between happiness score and contributing factors
- Ranking countries by score and analyzing trends
- Training predictive models (Linear Regression, Random Forest, Gradient Boosting) for happiness scoring

## Notes

This project is designed as an exploratory data analysis and modeling exercise. It is useful for understanding how different social and economic indicators relate to subjective well-being across countries over time.

## License

No explicit license file is included in this repository at this time.
