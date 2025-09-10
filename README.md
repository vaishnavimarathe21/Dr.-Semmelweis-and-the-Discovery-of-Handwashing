# Dr. Semmelweis and the Discovery of Handwashing

## Project Overview

This project analyzes the groundbreaking work of Dr. Ignaz Semmelweis, a Hungarian physician who discovered the importance of handwashing in preventing childbed fever in the 1840s. Through data analysis of mortality rates at Vienna General Hospital, this project demonstrates how statistical evidence could have supported Semmelweis' revolutionary medical discovery.

## Background

Dr. Ignaz Semmelweis (1818-1865) was a Hungarian physician working at Vienna General Hospital in the 1840s. He observed that women giving birth at the hospital were dying at an alarming rate from childbed fever (puerperal fever). Through careful observation and data collection, he discovered that the high mortality rates were caused by doctors who performed autopsies and then delivered babies without washing their hands.

## Dataset Description

The project uses two main datasets:

### 1. `yearly_deaths_by_clinic.csv`
- **Purpose**: Annual mortality data from 1841-1846
- **Columns**:
  - `year`: Year of data collection
  - `births`: Number of births
  - `deaths`: Number of deaths
  - `clinic`: Clinic identifier (clinic 1 or clinic 2)

### 2. `monthly_deaths.csv`
- **Purpose**: Monthly mortality data from 1841-1848
- **Columns**:
  - `date`: Date of data collection
  - `births`: Number of births
  - `deaths`: Number of deaths

## Key Findings

### 1. Alarming Mortality Rates
- **Clinic 1**: Consistently higher death rates (10%+ annually)
- **Clinic 2**: Lower death rates (2-4% annually)
- The difference was attributed to medical students (Clinic 1) vs. midwives (Clinic 2)

### 2. Impact of Handwashing
- **Before handwashing** (1841-1847): Average death rate ~10%
- **After handwashing** (1847-1848): Average death rate ~2%
- **Reduction**: Approximately 8 percentage points (80% reduction in mortality)

### 3. Statistical Significance
- Bootstrap analysis shows 95% confidence interval: 6.7% to 10% reduction
- Clear statistical evidence supporting handwashing effectiveness

## Analysis Methods

1. **Data Cleaning**: Processing mortality data and calculating proportions
2. **Visualization**: Line plots showing mortality trends over time
3. **Statistical Analysis**: Bootstrap confidence intervals for effect size
4. **Comparative Analysis**: Before vs. after handwashing implementation

## Historical Context

Despite having solid statistical evidence, Semmelweis faced significant resistance from the medical community:
- His theory was ridiculed by contemporary scientists
- He was forced to leave Vienna General Hospital in 1849
- The medical community largely rejected his discovery
- Statistics and statistical arguments were uncommon in 1800s medical science

## Technical Implementation

### Required Libraries
```python
import pandas as pd
import matplotlib.pyplot as plt
import numpy as np
```

### Key Code Snippets
- Data loading and preprocessing
- Proportion calculations
- Time series visualization
- Bootstrap analysis for confidence intervals

## Project Structure
```
Dr. Semmelweis and the Discovery of Handwashing/
├── datasets/
│   ├── yearly_deaths_by_clinic.csv
│   ├── monthly_deaths.csv
│   ├── ignaz_semmelweis_1860.jpeg
│   └── project_image.png
├── notebook.ipynb
└── README.md
```

## Learning Outcomes

This project demonstrates:
- Historical data analysis techniques
- Statistical methods for medical research
- Data visualization for trend analysis
- Bootstrap methodology for confidence intervals
- The importance of statistical evidence in scientific discovery

## Conclusion

Dr. Semmelweis' work represents one of the most important medical discoveries in history. This project shows how modern statistical analysis could have provided the evidence needed to convince the medical community of the importance of handwashing, potentially saving countless lives in the 19th century.

The analysis reveals that handwashing reduced childbed fever mortality by approximately 8 percentage points, with a 95% confidence interval of 6.7% to 10%. This represents a massive improvement in patient outcomes and demonstrates the power of data-driven medical practice.

## References

- Historical data from Vienna General Hospital
- Semmelweis' original research and observations
- Modern statistical analysis techniques
- Medical history of infection control practices
