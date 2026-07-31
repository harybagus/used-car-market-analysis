# Used Car Market Analysis (EDA & Data Wrangling)

## Project Overview

This project performs an end-to-end Exploratory Data Analysis (EDA) and data wrangling process on a large-scale dataset of US used car listings (~426k original records cleaned down to ~354k entries). The main objective is to clean contaminated secondary market data, analyze vehicle pricing dynamics, identify market supply dominance, and deliver actionable insights for automotive dealerships and listing platforms.

---

## Key Business Insights & Findings

1. **Market Supply Dominance:** US domestic automakers lead the used car inventory, headed by **Ford** (~70k units) and **Chevrolet** (~55k units), followed by major Japanese brands (**Toyota**, **Honda**, **Nissan**). **SUVs**, **Sedans**, and **Trucks** constitute the vast majority of available body types.
2. **Pricing & Depreciation:** The median used car price is **~$13,000**, with a strong negative correlation between `odometer` mileage and `price` (demonstrating a clear vehicle depreciation curve).
3. **Alternative Fuel Premiums:** Vehicles running on `diesel` and `electric` powertrains maintain higher resale values compared to standard gasoline cars.

---

## Data Wrangling & Preprocessing Highlights

- **Outlier Filtering:** Removed unrealistic price listings (< $500 or > $100,000) and extreme odometer readings (< 1,000 or > 300,000 miles).
- **Missing Value Strategy:** Dropped non-informative metadata (`county`, `url`, `image_url`) and imputed missing categorical features with `'unknown'`.
- **Data Quality:** Resolved dataset price anomalies and removed duplicate records, yielding a clean 354,198-row dataset ready for visual analysis.

---

## Business Recommendations

- **Inventory Sourcing:** Prioritize procurement of SUVs and Trucks with odometer readings below 100,000 miles to capture high market demand and ensure quicker inventory turnover.
- **Dynamic Pricing:** Capitalize on fuel-type premiums when pricing Diesel and Electric vehicles to maximize profit margins.
- **Data Quality Control:** Implement strict field validation on listing platforms to prevent placeholder values (e.g., $0 or $999,999 listings) from contaminating market data.

---

## Tech Stack & Tools

- **Language:** Python 3.x
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Environment:** Jupyter Notebook / Visual Studio Code
