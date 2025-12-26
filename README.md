# 🎵 Spotify Music Analytics Dashboard

Professional Power BI dashboard analyzing 8,774 tracks from 2,547 artists spanning 1960-2024.

![Dashboard Preview](documentation/screenshots/page1_executive.png)

## 📊 Project Overview

Interactive 4-page business intelligence dashboard built with Power BI Desktop, featuring:
- **Star Schema** data model (1 FACT table, 2 DIM tables)
- **Power Query** ETL transformations
- **15+ DAX** measures and calculated columns
- **Custom Spotify theme** (JSON)
- **Interactive filtering** by music genre

## 🎯 Key Features

### Page 1: Executive Overview
- High-level KPIs (tracks, artists, albums, popularity, duration)
- Top artists by track count
- Album type distribution

### Page 2: Artist Deep Dive
- Genre filtering (10 categories: Pop, Hip Hop, Rock, etc.)
- Artist ranking table (popularity, followers, tracks)
- Followers vs Popularity scatter plot

### Page 3: Content Analysis
- Explicit content distribution (75% Clean, 25% Explicit)
- Track duration histogram (peak at 3-4 minutes)

### Page 4: Timeline & Trends
- Dataset composition by release year (1960-2024)
- Albums per decade analysis
- Average duration stability over time

## 💡 Key Insights

- **75% Clean Content**: Spotify prioritizes family-friendly music
- **3.5 Min Sweet Spot**: Average track duration stable since 1960
- **Contemporary Focus**: 80% of dataset from 2010-2024
- **Taylor Swift Dominance**: 330 tracks (most prolific artist)

## 🛠️ Technologies

- Power BI Desktop
- Power Query (M language)
- DAX (Data Analysis Expressions)
- Star Schema modeling
- Custom JSON theming

## 📁 Repository Structure
```
spotify-powerbi-dashboard/
├── README.md
├── data/
│   └── track_data_final.csv          # Source dataset (8,774 tracks)
├── dashboard/
│   └── Spotify_Dashboard_v1.pbix     # Power BI file
├── theme/
│   └── Spotify_Dark_Theme.json       # Custom theme
└── documentation/
    ├── Spotify_Power_BI_Complete_Guide_v2.html
    └── screenshots/                   # Dashboard previews
        ├── page1_executive.png
        ├── page2_artists.png
        ├── page3_content.png
        └── page4_timeline.png
```

## 🚀 How to Use

1. **Download** the `.pbix` file from `dashboard/` folder
2. **Open** in Power BI Desktop (free download from Microsoft)
3. **Explore** 4 interactive pages
4. *Optional*: Apply custom theme from `theme/` folder

## 📈 Data Model

**Star Schema:**
```
FACT_Tracks (8,774 rows)
    ├── Relationships ──> DIM_Artists (2,549 unique artists)
    └── Relationships ──> DIM_Albums (5,317 unique albums)
```

**Transformations:**
- Power Query: Data cleaning, calculated columns (duration conversions, genre parsing)
- DAX: Aggregation measures (Total Tracks, Avg Popularity, etc.)
- Calculated columns: Decade grouping, Duration categories

## 📚 Documentation

Full step-by-step guide available in `documentation/Spotify_Power_BI_Complete_Guide_v2.html` covering:
- Star Schema design rationale
- Power Query transformations (M code)
- DAX formulas explained
- Visualization best practices
- Storytelling and insights interpretation

## 🎨 Design

Custom Spotify-themed design using official brand colors:
- Background: `#191414` (Spotify Black)
- Primary: `#1DB954` (Spotify Green)
- Text: `#FFFFFF` (White) / `#B3B3B3` (Gray)

## 🧠 Skills Demonstrated

- Data modeling (Star Schema, normalization)
- ETL processes (Power Query M)
- Business logic (DAX measures)
- Data visualization best practices
- Storytelling with data
- Understanding dataset limitations and bias

## ⚠️ Dataset Limitations

This dataset represents a **sample** of Spotify's catalog, not the entire platform:
- Biased toward contemporary/popular music
- Missing genres, independent artists, regional music
- Dataset composition ≠ global music production

Always interpret results as "in this dataset" rather than universal truths.

## 📝 License

This project is for educational and portfolio purposes.

## 👤 Author

**Marcin Banach**
- GitHub: [@mbimarban](https://github.com/mbimarban)

---

⭐ If you found this project helpful, please star this repository!
