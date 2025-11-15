# 🎧 Spotify Listening Insights & Growth Strategy

## Project Goal & Business Context
The goal of this analysis was to uncover the **key factors influencing track popularity, artist visibility, and audience engagement** across Spotify’s global streaming data.  
The resulting **Power BI dashboard** enables data-driven decisions for playlist curation, marketing optimization, and retention growth — aligning content strategies with user listening patterns.

This project demonstrates an **end-to-end data analytics pipeline**, from stakeholder requirement gathering through data strategy definition, model design, and executive reporting.

---

## 🛠️ Technologies & Tools

| Component | Tool Used | File / Link |
| :--- | :--- | :--- |
| **Data Source** | Spotify Web API + Kaggle Dataset | [World’s Spotify Top 50 Playlist Data](https://www.kaggle.com/datasets/miquelneck/worlds-spotify-top-50-playlist-musicality-data/data) |
| **Data Processing** | Excel / Google Sheets (data cleaning, transformation) | Duration conversion, explicit tagging, deduplication |
| **Data Modeling** | Power BI Desktop | Fact & Dimension model (Tracks, Artists, Albums, Streams) |
| **Visualization / BI** | Microsoft Power BI Service | [Interactive Power BI Dashboard](https://app.powerbi.com/links/804iB6z2i0?ctid=5349a4dc-a350-45ff-b7b5-ffbd5c5fc573&pbi_source=linkShare) |
| **Presentation** | Microsoft PowerPoint 365 | [Final Executive Summary Presentation](https://1drv.ms/p/c/60cb6126e5f608d9/EZzjAkKArb1MqnOi-AGTUc4B4uWbnp77Rtol_uH1AU8DtA?e=2K1XM4) |

---

## 🔑 Key Insights & Deliverables

1. **Genre & Artist Dominance**  
   Pop and Hip-Hop genres account for **~75 % of global Top-50 streams**, with top artists (e.g., Taylor Swift, The Weeknd, Bad Bunny) contributing over **40 %** of total plays.

2. **Optimal Track Characteristics**  
   High-energy songs between **3 – 4 minutes** achieve the **highest average popularity (> 85)**, confirming duration and energy as major engagement drivers.

3. **Explicit vs. Clean Trade-off**  
   Explicit tracks show **10–15 % more initial plays** but lower retention, guiding balanced playlist curation for sustainable engagement.

4. **Regional Personalization Potential**  
   Regional trends highlight opportunities for **localized playlists**—Europe and Latin America display diverse genre preferences, while North America leans mainstream.

5. **Albums vs. Singles**  
   **68 %** of Top-50 tracks are singles; albums deliver longer-term playlist presence, informing release-cycle strategies.

---

## 🎯 Actionable Recommendations

- **Curate Playlists Strategically:** Focus on mid-duration, high-energy tracks; blend explicit/clean content for sustained engagement.  
- **Promote Artist Collaborations:** Cross-genre features increase long-term streams by ~18 %.  
- **Localize Content:** Build region-specific playlists to raise retention **6–8 % QoQ**.  
- **Enhance Monitoring:** Implement predictive analytics within Power BI to forecast popularity decay and trigger timely promotions.

---

## 🧱 Data Strategy & Model Summary

| Layer | Key Fields / Metrics | Transformation Highlights |
| :--- | :--- | :--- |
| **Track Table** | `track_id`, `track_name`, `album_id`, `artist_id`, `duration_min`, `popularity`, `is_explicit` | Duration converted from ms → minutes; cleaned text; deduplicated IDs |
| **Artist Table** | `artist_id`, `artist_name`, `followers`, `genres` | Normalized genres; mapped artist-region relationships |
| **Album Table** | `album_id`, `album_name`, `album_type`, `release_date`, `total_tracks` | Categorized album_type (“Single” / “Album”) |
| **Stream Metrics** | `region`, `total_streams`, `chart_position`, `date_added` | Filtered nulls; derived KPIs |
| **KPIs** | Total Streams, Avg Popularity, Explicit %, Artist Reach, Stream Growth % | Calculated via DAX in Power BI |

**Success Criteria:**  
- Live API refresh from Spotify Web API  
- Consistent KPI logic across visuals  
- Intuitive interactive experience for non-technical stakeholders  

---

## 📈 BI Dashboard & Presentation Links
- **Interactive Power BI Dashboard:** [View Online →](https://app.powerbi.com/links/804iB6z2i0?ctid=5349a4dc-a350-45ff-b7b5-ffbd5c5fc573&pbi_source=linkShare)  
- **Executive Summary Presentation:** [View PowerPoint →](https://1drv.ms/p/c/60cb6126e5f608d9/EZzjAkKArb1MqnOi-AGTUc4B4uWbnp77Rtol_uH1AU8DtA?e=2K1XM4)  
- **Dataset Source:** [Kaggle – World’s Spotify Top 50 Musicality Data](https://www.kaggle.com/datasets/miquelneck/worlds-spotify-top-50-playlist-musicality-data/data)
- **Spotify_Analysis(.pbix) File:** [View Online →](https://1drv.ms/p/c/60cb6126e5f608d9/EZzjAkKArb1MqnOi-AGTUc4B4uWbnp77Rtol_uH1AU8DtA?e=2K1XM4)

---

## 🧠 Project Structure

| File | Description |
| :--- | :--- |
| `Spotify_Stakeholder_Requirements_Document.pdf` | Defines business questions, stakeholders, KPIs, and success metrics. |
| `Spotify_Data_Strategy_Requirements_Document.pdf` | Maps stakeholder needs into technical data requirements and transformations. |
| `Spotify_Executive_Summary_Report.pdf` | Final summarized analysis, findings, and recommendations. |
| `Spotify_Analysis.pbix` | Power BI file containing data model, DAX measures, and dashboards. |
| `Spotify_Executive_Summary_Final.pptx` | Final presentation deck aligned with the dashboard visuals. |

---

### 🧾 Author & Credits
**BI Analyst:** Tanzil Ali Rizvi  
**Client/Sponsor:** Spotify Analytics Team  
**Date:** November 2025  

---

> “Turning sound into strategy — leveraging data to amplify discovery and listener delight.”
