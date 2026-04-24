# London Airbnb Analysis

An end-to-end data analysis project using real London Airbnb data from Inside Airbnb (September 2025). This project covers the full data pipeline from raw data through to a dashboard.

---

## Project outline

### 1. Data wrangling (`notebooks/01_data_wrangling.ipynb`)
- Load listings, reviews, neighbourhoods and GeoJSON data
- Identify and handle missing values
- Clean the price column
- Remove invalid listings
- Save cleaned data ready for analysis

### 2. Exploratory Data Analysis (`notebooks/02_EDA.ipynb`)
- Price distribution across London
- Average price by neighbourhood
- Room type breakdown
- Superhost vs regular host comparison
- Availability trends
- Geographic price map by neighbourhood

### 3. SQL Analysis (`notebooks/03_SQL.ipynb`)
- Load cleaned data into SQLite database
- Query average price by neighbourhood
- Compare superhost vs regular host pricing
- Find most reviewed listings
- Analyse review trends over time

### 4. Sentiment Analysis (`notebooks/04_sentiment.ipynb`)
- Sample reviews for analysis
- Run TextBlob sentiment scoring on review comments
- Classify each review as positive, neutral or negative
- Compare sentiment by neighbourhood
- Find most common words in positive vs negative reviews

### 5. Predictive Modelling (`notebooks/05_modelling.ipynb`)
- Regression model to predict listing price
- Classification model to identify good value listings
- Feature importance analysis
- Model evaluation

### 6. Dashboard
- Interactive dashboard built in Tableau
- Key insights from the analysis
- Geographic map of London listings

---

## Dataset

Source: [Inside Airbnb](http://insideairbnb.com/get-the-data) — London, September 2025

| File | Description |
|---|---|
| `listings.csv.gz` | Detailed listing data (79 columns) |
| `reviews.csv.gz` | Guest reviews with comment text |
| `neighbourhoods.csv` | London neighbourhood list |
| `neighbourhoods.geojson` | Geographic boundaries for mapping |

> Data files are not included in this repo — download from Inside Airbnb and place in the `data/` folder.

---

## Key findings



---

## Project structure

```
airbnb-london-analysis/
├── notebooks/
│   ├── 01_data_wrangling.ipynb
│   ├── 02_EDA.ipynb
│   ├── 03_SQL.ipynb
│   ├── 04_sentiment.ipynb
│   └── 05_modelling.ipynb
├── data/                  # not tracked in git
├── sql/                   # SQL query files
├── dashboard/             # dashboard screenshots
├── .gitignore
└── README.md
```

---

## Tech stack

| Tool | Purpose |
|---|---|
| Python | Data analysis |
| Pandas | Data wrangling |
| Matplotlib / Seaborn | Visualisation |
| SQLite | SQL analysis |
| TextBlob | Sentiment analysis |
| Scikit-learn | Predictive modelling |
| Folium | Geographic mapping |
| Tableau | Dashboard |

---

## License

MIT
