# Video Game Sales — Data Cleaning Project

## Results

| Metric | Before | After |
|---|---|---|
| Total Rows | 16,598 | 16,287 |
| Missing Values | 329 | 0 |
| Year dtype | float64 | int64 |
| Duplicate Rows | 0 | 0 |

## Cleaning Decisions

- **Year (271 missing):** Dropped — release year cannot be reliably guessed
- **Year (4 post-2016):** Dropped — dataset scraped in 2016, sales data unreliable  
- **Year dtype:** Converted float64 → int64 after nulls removed
- **Publisher (36 missing):** Dropped — only 0.22% of data, publisher identity unverifiable
- **Global Sales mismatch:** No action — confirmed floating point rounding artifact, max difference 0.02M

  ## Dataset
[Video Game Sales — Kaggle](https://www.kaggle.com/datasets/gregorut/videogamesales)
