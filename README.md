# Music Taste Analysis: Springfield vs. Shelbyville

## Project Overview

This project analyzes a dataset of music tracks streamed in two fictional cities, Springfield and Shelbyville. The goal is to understand and compare their music preferences, test hypotheses about listening behavior, and practice data wrangling and visualization techniques.

This project was conducted as an enhancement of a bootcamp assignment to showcase skills in data cleaning, exploratory data analysis (EDA), and hypothesis testing using Python, Pandas, and Matplotlib/Seaborn.

---

## Key Questions

1.  What are the most popular music genres in Springfield and Shelbyville?
2.  How do the music tastes of the two cities compare?
3.  Does listening behavior change significantly between Monday and Friday?

---

## Data Source

The dataset is a CSV file named `music_project_en (1).csv` containing the following columns:
* `userID`: A unique identifier for the user.
* `Track`: The name of the song.
* `artist`: The name of the artist.
* `genre`: The genre of the track.
* `City`: The city where the track was played (Springfield or Shelbyville).
* `time`: The exact time the track was played.
* `day`: The day of the week the track was played.

---

## Methodology

1.  **Data Cleaning:**
    * Standardized column headers (lowercase and no spaces).
    * Handled missing values in `track`, `artist`, and `genre` by filling them with 'unknown'.
    * Removed 3,826 duplicate rows.
    * Corrected implicit duplicates in the `genre` column (e.g., merging 'hip-hop' and 'hiphop').

2.  **Exploratory Data Analysis (EDA):**
    * Compared total listening counts for both cities.
    * Visualized and compared the top 10 genres in each city.

3.  **Hypothesis Testing:**
    * Analyzed and visualized the top genres for Mondays and Fridays to determine if listening habits change significantly during the week.

---

## Key Findings

* Springfield has significantly more listening activity than Shelbyville.
* Both cities share the same top 4 favorite genres: **Pop, Dance, Rock, and Electronic**.
* The primary difference in taste is in niche genres. Springfield prefers **Classical** and **World** music, while Shelbyville shows a stronger preference for **Alternative** music.
* The hypothesis that music taste changes from Monday to Friday was **not supported** by the data. Listening patterns remained remarkably consistent in both cities.

---

## How to Reproduce

To run this analysis yourself, clone the repository, install the required packages, and run the `music_analysis.ipynb` notebook:

```bash
git clone [YOUR_GITHUB_REPO_URL]
cd music-taste-analysis
pip install -r requirements.txt
jupyter notebook music_analysis.ipynb
```

---
## Tools Used
* Python
* Pandas
* Matplotlib
* Seaborn
* Jupyter Notebook