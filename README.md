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
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy
- Jupyter Notebook

## Setup

```bash
git clone https://github.com/BrianCao10/Word-Happiness-Analysis.git
cd Word-Happiness-Analysis
python -m venv .venv
source .venv/bin/activate
pip install jupyter pandas numpy matplotlib seaborn scipy scikit-learn
```

## Run the Notebook

```bash
jupyter notebook World_Happiness.ipynb
```
## Conclusions

**1. Happiness is broadly stable, with a modest upward drift.**
Global mean and median happiness scores dipped in 2017 but rose overall
between 2015 and 2019, with the median improving more than the mean. This
suggests gains were concentrated in the middle of the distribution rather
than driven by a few extreme countries.

**2. Economic and health indicators have the strongest link to happiness.**
GDP per capita (r = 0.79) and healthy life expectancy (r = 0.74) had the
strongest correlations with score, followed by social support (0.65) and
freedom (0.55). Perceptions of corruption were moderate (0.40), and
generosity was weak (0.14), so generosity says little about a country's
overall ranking.

**3. The top of the rankings is very stable.**
New Zealand, Australia, Iceland, Denmark, and the Netherlands varied by
only a few positions across five years. Top-ranked countries tend to stay
there, so large shifts at the top are rare.

**4. The biggest movement happens in the middle and lower ranks.**
Benin (+53 places), Ivory Coast (+52), Honduras (+46), Hungary (+42), and
Gabon (+39) improved the most from 2015 to 2019. Rankings are far more
volatile outside the top tier, so small score changes there can mean large
rank changes.

**5. A simple weighted index tracks the official score closely.**
A custom index built from just four factors (GDP, support, freedom, health)
correlated 0.86 with the official score, suggesting a handful of indicators
capture most of what the full methodology measures.

## Recommendations

- **Look at the climbers.** Benin, Ivory Coast, Honduras, Hungary, and Gabon
  are good case studies for what changed, such as policy, economic, or
  health developments. This analysis can't identify the cause, but it
  shows where to look.
- **Prioritize health and economic indicators when comparing countries.**
  They explain the most variation, while generosity adds little.
- **Interpret rank changes cautiously.** Because the middle of the table is
  tightly packed, a small score change can move a country many places.

## Limitations

- Correlation does not imply causation.
- The scores come from self-reported surveys and may be affected by
  cultural differences in how people answer.
- GDP, health, and social support likely overlap with each other, so their
  individual effects can't be cleanly separated.
- The same countries appear in all five years, so observations aren't
  fully independent.
- Findings cover 2015-2019 only and don't capture later events.
