# Streaming Platform Content Strategy Analysis

## 📌 Project Scope
This project focuses on content strategy analysis for streaming platforms.
Netflix content data is used as a primary case study to analyze content growth, genre distribution, regional presence, and audience targeting strategies.

## 📊 Project Overview
This project analyzes streaming platform content data to understand how content has evolved over time, how it is distributed across regions, and what kind of audience it targets.

The goal was to build a complete analytics workflow — starting from raw data, cleaning and transforming it, validating results, and finally presenting insights using dashboards.

---

## Tech Stack
- Python (pandas, numpy, matplotlib)
- Excel (Pivot Tables, Power Query)
- Power BI

---

## Dataset
Each row represents a single title available on the platform (movie or TV show).

Main fields used:
- title  
- Type (Movie / TV Show)  
- release_year  
- rating (PG, TV-MA, etc.)  
- country  

Some fields, like country, contain multiple values and required normalization before analysis.

---

## Data Preparation
The raw dataset was cleaned and prepared in Python:
- removed and handled missing values
- split multi-country entries and normalized them
- created additional features based on release year to classify content as:
  - Legacy (before 2000)
  - Not Recent (2000–2014)
  - Recent (2015 onwards)

Cleaned data was exported and validated in Excel before visualization.

---

## Analysis Performed
The following questions were explored:
- How many movies vs TV shows are available?
- How has content production changed over the years?
- Which countries contribute the most content?
- What audience maturity ratings dominate the platform?
- How much of the catalog is recent vs older content?

---

## 🔍 Exploratory Analysis
Matplotlib was used during the exploratory phase to quickly validate trends, distributions, and data quality before building final reports and dashboards.

## 📊 Excel-Based Analysis
Excel was used to:
- Build pivot tables for key summary metrics
- Normalize country data using Power Query
- Validate results generated in Python
- Perform quick visual checks for trends and distributions

## 📈 Power BI Dashboard
An interactive Power BI dashboard was developed to present insights, with slicers for:
- Year
- Country
- Content type (Movie / TV Show)
- Content age category (Recent / Old / Vintage)

The dashboard emphasizes clarity, interpretability, and analytical value over decorative visuals.

## 📌 Key Takeaways
- Content production increased sharply after 2015
- TV shows have grown faster than movies in recent years
- The United States and India are the largest content-producing countries
- Most content targets mature audience ratings
- Recent content accounts for the majority of the catalog

---

## Project Structure
```
streaming_platform_content_strategy_analysis/
├── data/
├── notebooks/
├── excel/
├── powerbi/
├── images/
└── README.md
```


---

## Notes
This project is platform-agnostic. Netflix was used as the sample dataset, but the same approach can be applied to other streaming services.
