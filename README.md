# World Happiness Analysis

This repository analyzes World Happiness Report data from 2015 to 2019 and combines the yearly datasets into a unified dataset for comparison and modeling.

## Project Overview

The notebook explores which factors are most strongly associated with a country's happiness score, including GDP per capita, social support, health, freedom, trust, and generosity.

## Key Findings

- Nordic countries such as Finland, Denmark, Norway, Iceland, and Switzerland consistently rank near the top.
- GDP is important, but social support, health, and freedom are also major drivers of happiness.
- Countries with lower happiness scores tend to have weaker economies, lower life expectancy, and reduced social stability.
- Happiness is best explained by a combination of economic and social well-being indicators, not by one factor alone.
- The notebook also tests predictive models to estimate happiness from these variables.

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

## Technologies Used

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- SciPy
- Jupyter Notebook

## Setup

```bash
git clone https://github.com/Brian-Cao10/Word-Happiness-Analysis.git
cd Word-Happiness-Analysis
python -m venv .venv
source .venv/bin/activate
pip install jupyter pandas numpy matplotlib seaborn scipy scikit-learn
```

## Run the Notebook

```bash
jupyter notebook World_Happiness.ipynb
```

## Notes

This project is an exploratory data analysis and modeling exercise focused on understanding how socioeconomic indicators relate to well-being across countries and years.
