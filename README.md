# London Airbnb Analysis

A data analysis project looking at Airbnb listings in London using data from Inside Airbnb (September 2025). The project goes from raw data all the way through to an interactive dashboard.

**[View the Tableau Dashboard](https://public.tableau.com/app/profile/dania.quazi/viz/LondonAirbnbAnalysis_17771151962090/LondonAirbnbDashboard)**

---

## What's in this project

### 1. Data Wrangling (`notebooks/01_data_wrangling.ipynb`)
- Load the listings, reviews and neighbourhood data
- Fix missing values
- Clean the price column
- Remove listings with bad or missing data
- Save the cleaned data

### 2. Exploratory Data Analysis (`notebooks/02_EDA.ipynb`)
- Look at how prices are spread across London
- Find the most and least expensive neighbourhoods
- Break down listings by room type
- Compare superhost and regular host listings
- Look at availability patterns

### 3. SQL Analysis (`notebooks/03_SQL.ipynb`)
- Load the data into a SQLite database
- Write SQL queries to answer questions about price, superhosts and reviews

### 4. Sentiment Analysis — TextBlob (`notebooks/04_sentiment_textblob.ipynb`)
- Score guest reviews using TextBlob
- Label each review as positive, neutral or negative
- Look at which neighbourhoods get the best reviews

### 5. Sentiment Analysis — VADER (`notebooks/05_sentiment_vader.ipynb`)
- Score the same reviews using VADER
- Compare results with TextBlob
- Visualise the overall sentiment breakdown

### 6. Modelling (`notebooks/06_modelling.ipynb`)
- Build a model to predict listing price
- Look at which factors matter most for price
- Evaluate how well the model performs

### 7. Dashboard
- Built in Tableau Public
- Map showing average price by London borough
- Price distribution chart
- Room type comparison
- Superhost vs non-superhost comparison
- Sentiment breakdown

---

## Key Findings

- Central London (Westminster, Kensington & Chelsea) has the highest average prices
- Most listings are entire homes, which are also the most expensive
- Superhosts tend to get better reviews but charge similar prices
- More than 85% of reviews are positive
- Most listings cost between £50 and £150 per night

---

## Data

Source: [Inside Airbnb](http://insideairbnb.com/get-the-data) — London, September 2025

| File | Description |
|---|---|
| `listings.csv.gz` | Full listing data |
| `reviews.csv.gz` | Guest reviews |
| `neighbourhoods.csv` | List of London neighbourhoods |
| `neighbourhoods.geojson` | Borough boundaries for mapping |

> Data files are not included in this repo. Download from Inside Airbnb and put them in the `data/` folder.

---

## Project Structure

```
airbnb-london-analysis/
├── notebooks/
│   ├── 01_data_wrangling.ipynb
│   ├── 02_EDA.ipynb
│   ├── 03_SQL.ipynb
│   ├── 04_sentiment_textblob.ipynb
│   ├── 05_sentiment_vader.ipynb
│   └── 06_modelling.ipynb
├── data/                  # not tracked in git
├── .gitignore
└── README.md
```

---

## Tools Used

| Tool | What it was used for |
|---|---|
| Python | Main analysis language |
| Pandas | Data cleaning and analysis |
| Matplotlib / Seaborn | Charts and graphs |
| SQLite | SQL queries |
| TextBlob | Sentiment analysis |
| VADER | Sentiment analysis |
| Scikit-learn | Price prediction model |
| Tableau Public | Interactive dashboard |

---

## License

MIT
