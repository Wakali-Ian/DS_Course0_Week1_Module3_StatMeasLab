# Statistical Measures Lab: Widget Sales

Flatiron Data Science, Course 0, Week 1, Module 3.

## Overview

This lab applies measures of central tendency and dispersion in Python to summarize a year of widget sales and advertising spend across 200 markets. The analysis answers three business questions:

1. What has been the typical sales volume across markets?
2. How variable have sales been across markets?
3. How much has the company characteristically spent on TV, radio, and newspaper advertising?

## Dataset

`Advertising.csv` has 200 rows (one per market) and these columns:

| Column | Description |
|---|---|
| `sales` | Widgets sold (thousands) |
| `TV` | TV ad spend (thousands of dollars) |
| `radio` | Radio ad spend (thousands of dollars) |
| `newspaper` | Newspaper ad spend (thousands of dollars) |

The first column is an unnamed row index.

## Results

| Measure | Value |
|---|---|
| Number of markets | 200 |
| Sales range | 1.6 to 27.0 thousand widgets |
| Typical sales (mean) | 14.02 thousand widgets |
| Sales dispersion (standard deviation) | 5.20 |

| Medium | Median spend ($ thousands) | IQR ($ thousands) |
|---|---|---|
| TV | 149.75 | 144.45 |
| Radio | 22.90 | 26.55 |
| Newspaper | 25.75 | 32.35 |

The sales histogram is roughly bell-shaped with a slight right skew (skewness about 0.40), so the mean and standard deviation describe it well. Ad spend is summarized with the median and IQR, which are less sensitive to outliers.

## Skills Practiced

- Loading a CSV with `csv.DictReader`
- Extracting columns into lists
- Computing min, max, mean, median, standard deviation, and IQR
- Choosing a measure of central tendency and dispersion from a histogram

## Files

- `DS_Course0_Week1_Module3_StatMeas.ipynb`: the completed lab notebook
- `Advertising.csv`: the dataset
- `README.md`: this file

## How to Run

```bash
conda activate learn-env
jupyter notebook
```

Open `DS_Course0_Week1_Module3_StatMeas.ipynb` and choose **Kernel > Restart & Run All**.

Requires Python 3 with `numpy`, `scipy`, and `matplotlib`.

## Author

Ian Stephen Wakali ([Wakali-Ian](https://github.com/Wakali-Ian))
