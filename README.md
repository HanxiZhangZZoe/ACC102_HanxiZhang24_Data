# ACC102_HanxiZhang24_Data
# K-Pop Industry Data Analysis

## 1. Problem & User
This project analyzes the historical trajectory, market saturation, and survival models of K-Pop groups. The analytical tool is designed for entertainment industry executives, media investors, and strategic analysts seeking data-driven insights into market entry feasibility, competitive density, and agency dominance.

## 2. Data
**Source:** `kpopgroups.csv` (stored in `/data` directory of this repository)
**Access Date:** April 2026
**Key Fields Used:** Group Name, Gender, Debut Date, Company, Original Members, Current Members, Active Status

## 3. Methods
The analytical workflow is strictly Python-based:
**Data Cleaning:** Used `pandas` to handle NaN values, parse string dates to datetime, and enforce integer constraints.
**Feature Engineering:** Calculated `Retention_Rate` and created `Agency_Tier` classification based on production volume.
**Visualization:** Used `plotly.express` with `plotly_dark` template to generate interactive, high-fidelity charts.

## 4. Key Findings
**Market Boom & Saturation:** A significant surge in group debuts occurred over the last decade, indicating severe market saturation.
**"Tier 1" Dominance:** A highly concentrated number of top-tier agencies (SM, JYP, YG) dominate market output, showcasing a strong "Matthew Effect" in K-Pop.
**Gender & Survival Dynamics:** Male groups have a ~75% survival rate, compared to ~52% for female groups, suggesting differences in long-term active status.

## 5. How to Run
To ensure full reproducibility:
1. Clone this repository to your local machine
2. Install dependencies: `pip install pandas numpy plotly`
3. Open `analysis.ipynb` in Jupyter environment
4. Run all cells sequentially (data will be loaded from `/data/kpopgroups.csv`)

## 6. Limitations & Next Steps
**Limitations:** The dataset relies on static historical data; it does not include financial metrics, exact disbandment dates, or real-time social media popularity.
**Next Steps:** Future work could incorporate web scraping for real-time sentiment analysis or merge financial data to build predictive models for group profitability.
