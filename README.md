# Video Game Sales — Data Analysis Project

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

## Analysis
- Post-cleaning the data I analysed it using Python Libraries (Matplotlib + Seaborn)
- 5 visualisation produced understanding the varied nature of sales patterns across ***Publishers, Platforms ,Regions & Time***

### Major Key Findings
1. Nintendo has a clear lead amongst other publishers (1750 + million sales) almost double of Electronic Arts.

2. Sales peaked during 2008-2009 mainly due to wii.Decline post-2010 show the global market shifting from physical media to digital media contrary to the belief that the industry was shrinking it was changing.
3. NA & EU follow identical trends across decades showing identical peaks and troughs with sales in NA being twice of that in EU.
4. Japan's record-sales being in Role-playing games shows the culture's appreciation for story-driven games unlike North American and European sales which show the cultural appreaciation for Sports
5. PS2 supermacy despite launching in 2000.PS2's closest rivals were the 7th generation trio (PS3/X360/Wii) 
which fought the closest three-way console competition in history — 
yet none matched PS2's total.

## Files
| File | Description |
|---|---|
| `cleaning.ipynb` | Data cleaning pipeline |
| `analysis.ipynb` | Exploratory analysis + visualisations |
| `data/cleaned/vgsales_clean.csv` | Final cleaned dataset |
