# Netflix-Data-Analysis

A complete Exploratory Data Analysis (EDA) project on a Netflix-style content dataset, uncovering trends across genres, countries, ratings, viewership, and content type using Python.

## 📌 Project Overview

This project analyzes a dataset of 100 Netflix titles (Movies and TV Shows) to answer key business questions such as:

- What type of content dominates the platform — Movies or TV Shows?
- Which genres and countries produce the most content?
- How are ratings and viewership distributed?
- Which titles perform best in terms of rating and views?
- Is there a relationship between rating, duration, and views?

The analysis follows a structured EDA workflow: data loading → cleaning/validation → univariate analysis → bivariate analysis → correlation analysis → key insights.

## 📂 Dataset

**File:** `netflix_dataset.csv`

| Column | Description |
|---|---|
| `show_id` | Unique identifier for each title |
| `title` | Name of the movie/show |
| `type` | Content type — Movie or TV Show |
| `release_year` | Year the content was released |
| `genre` | Genre category |
| `country` | Country of origin |
| `rating` | Average user rating (0–10) |
| `duration_min` | Duration in minutes |
| `views_millions` | Total views (in millions) |

**Shape:** 100 rows × 9 columns
**Missing values:** None
**Duplicate rows:** None

## 🛠️ Tools & Libraries

- **Python 3**
- **Pandas** – data loading, cleaning, and aggregation
- **Matplotlib** – data visualization
- **Jupyter Notebook** – interactive analysis environment

## 🔍 Analysis Performed

1. **Data Inspection** — shape, columns, data types, null checks, duplicate checks, statistical summary
2. **Content Type Distribution** — Movies vs TV Shows
3. **Genre Distribution** — count of titles per genre
4. **Country Distribution** — content spread across countries
5. **Rating Distribution** — histogram of rating values
6. **Duration Distribution** — histogram of runtime
7. **Release Year Trend** — number of titles released per year
8. **Top 10 Most Viewed Titles**
9. **Top 10 Highest Rated Titles**
10. **Average Rating by Genre**
11. **Average Views by Genre**
12. **Correlation Analysis** — rating vs. duration vs. views
13. **Rating vs. Views Scatter Plot**
14. **Extreme Value Lookups** — highest rated, longest duration, most viewed title

## 📊 Key Insights

- **Content mix:** Movies (56%) slightly outnumber TV Shows (44%).
- **Top genre:** Documentary is the most common genre (17 titles), followed closely by Thriller (16).
- **Top country:** The USA leads content production (21 titles), followed by the UK (18) and Japan (16).
- **Average rating:** 7.21 / 10, with Thriller having the highest average rating (7.66) among genres.
- **Average views:** ~128.8M per title, with Documentary and Sci-Fi genres driving the highest average views.
- **No strong correlation** was found between rating, duration, and views (all correlation coefficients close to 0) — meaning higher-rated or longer content doesn't necessarily translate to more views.
- **Most viewed title:** "Netflix Title 45" with 249.6M views, despite only a 5.0 rating — showing popularity isn't rating-driven.
- **Highest rated title:** "Netflix Title 16" with a 9.5 rating.

## 📈 Sample Visualizations

The notebook generates the following charts:
- Bar chart — Movies vs TV Shows
- Bar chart — Genre distribution
- Bar chart — Country distribution
- Histogram — Rating distribution
- Histogram — Duration distribution
- Line chart — Release year trend
- Bar chart — Top 10 most viewed titles
- Bar chart — Average rating by genre
- Bar chart — Average views by genre
- Scatter plot — Rating vs. Views

## 🚀 How to Run

1. Clone this repository
   ```bash
   git clone https://github.com/nikhil-manihal16/netflix-content-analysis.git
   cd netflix-content-analysis
   ```
2. Install dependencies
   ```bash
   pip install pandas matplotlib jupyter
   ```
3. Launch the notebook
   ```bash
   jupyter notebook notebook.ipynb
   ```
4. Run all cells to reproduce the analysis and visualizations.

## 📁 Project Structure

```
netflix-content-analysis/
│
├── netflix_dataset.csv     # Raw dataset
├── notebook.ipynb          # EDA notebook with analysis & visualizations
└── README.md                # Project documentation
```

## 🔮 Future Improvements

- Add interactive dashboards using Plotly or Power BI
- Perform time-series forecasting on content release trends
- Build a genre/country-based recommendation logic
- Segment analysis by release decade

## 👤 Author

**Nikhil**
Aspiring Data Analyst | Python • SQL • Data Visualization
📫 Connect on [LinkedIn](https://linkedin.com)

## 📄 License

This project is open-sourced under the [MIT License](LICENSE).
