# Netflix Data Analysis 🎬

A data analysis project exploring Netflix's content library - what they have, where it comes from, and how their catalog has evolved over time.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Status](https://img.shields.io/badge/Status-Complete-green.svg)

## What's This About?

I was curious about Netflix's content strategy, so I grabbed a dataset of their titles and started digging. Turns out there are some interesting patterns in how they build their library.

**Some questions I wanted to answer:**
- How's the movie vs TV show split?
- Which countries produce the most content?
- When did Netflix really start growing their library?
- What day do they usually drop new content?

## Quick Findings

| Metric | Value |
|--------|-------|
| Total Titles | 8,790 |
| Movies | 6,126 (70%) |
| TV Shows | 2,664 (30%) |
| Countries | 86 |
| Date Range | 2008-2021 |

**The interesting bits:**
- US makes 37% of the content, India is second with 12%
- TV-MA (mature audiences) is by far the most common rating
- Friday is THE release day - they know we're planning our weekend binges
- 2019 was peak content addition year
- Most TV shows only have 1 season

## Sample Visualizations

### Content Distribution
![Content Type](visualizations/01_content_type.png)

### Growth Over Time
![Yearly Growth](visualizations/04_yearly_growth.png)

### Dashboard Overview
![Dashboard](visualizations/00_dashboard.png)

## Project Structure

```
netflix-analysis/
├── Netflix_Data_Analysis.ipynb   # main analysis notebook
├── netflix1.csv                  # original dataset
├── README.md                     # you're here
├── requirements.txt              # dependencies
├── data/
│   └── netflix_cleaned.csv       # cleaned dataset
└── visualizations/               # all the charts
    ├── 00_dashboard.png
    ├── 01_content_type.png
    ├── 02_ratings.png
    ├── 03_top_countries.png
    ├── 04_yearly_growth.png
    ├── 05_monthly_pattern.png
    ├── 06_movie_genres.png
    ├── 07_tvshow_genres.png
    ├── 08_top_directors.png
    ├── 09_movie_duration.png
    ├── 10_tvshow_seasons.png
    ├── 11_release_year.png
    ├── 12_title_words.png
    ├── 13_rating_heatmap.png
    └── 14_day_of_week.png
```

## How to Run

1. Clone this repo
```bash
git clone https://github.com/yourusername/netflix-analysis.git
cd netflix-analysis
```

2. Install requirements
```bash
pip install -r requirements.txt
```

3. Open the notebook
```bash
jupyter notebook Netflix_Data_Analysis.ipynb
```

4. Run all cells - it'll generate the cleaned data and all visualizations automatically

## Tech Stack

- **Python 3.8+**
- **Pandas** - data wrangling
- **Matplotlib & Seaborn** - visualizations
- **Jupyter Notebook** - analysis environment

## Dataset

The dataset contains Netflix titles added between 2008-2021 with info like:
- Title, type (movie/show)
- Director, country
- Date added, release year
- Rating, duration
- Genre categories

## What I Learned

This was a good exercise in:
- Cleaning messy date formats
- Creating meaningful visualizations
- Finding patterns in categorical data
- Building a dashboard summary

## Future Ideas

Some things I might explore later:
- Sentiment analysis on titles/descriptions
- Building a simple recommendation system
- Comparing with other streaming platforms
- Predicting what makes content successful

---

Feel free to fork this and play around with it. If you find something interesting, let me know!
