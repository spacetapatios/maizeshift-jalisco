# 🌽 MaizeShift Jalisco

**A decision-support tool to explore crop rotations in Jalisco, Mexico.**

Developed for the **NASA Space Apps Challenge 2026** - Challenge: *Field Shift: Adapting Farms with NASA Data*.

👉 **[Click here to test the live application (GitHub Pages)](https://spacetapatios.github.io/maizeshift-jalisco/)**

---

## 📖 Overview

Farmers in Jalisco face shifting temperatures, unpredictable rainfall patterns, and water shortages. MaizeShift combines NASA climate and soil-wetness data with the farmer's priorities to suggest crop rotation strategies that can strengthen soil health and adapt their farms to changing conditions.

## 🚀 Key Features

*   **Historical Climate Analysis:** Uses **NASA POWER** data (1995-2025) to show trends in temperature, precipitation, and extreme heat days.
*   **Rotation Explorer:** Allows the farmer to select their priorities (water conservation, soil health, etc.) and compares different rotation strategies, including the existing crop rotation.
*   **Interactive Map:** Displays maize regions in Jalisco to contextualize the data.
*   **Farmer-Centered Design:** Simple language interface designed to be interpreted by users who may have limited technical or geospatial experience.

## 🔬 Methodology & Data

*   **Data Source:** NASA POWER (2 m air temperature, bias-corrected precipitation, root-zone soil wetness, and daily maximum temperature).
*   **Processing:** Data is fetched live for each region's coordinates. The growing season is defined as June–October. 
*   **Model:** The rotation explorer calculates water supply (season rain + usable soil water + irrigation) and heat pressure to evaluate crops. Scores are weighted by the farmer’s priorities.
*   **Maps:** Current conditions in map popups are from Open-Meteo. Satellite imagery and place names are from Esri.

## ⚠️ Limitations & Transparency

*   This tool is **not a yield forecast**. It provides signals to support decisions, to be combined with local agronomic advice.
*   Crop and soil values are simplified, illustrative assumptions (typical ranges); they are meant to be replaced with local data and agronomist input.
*   Uses one grid point per region (cells of about 0.5° × 0.625°); no yield or irrigation data is included.
*   **The tool is designed to support—not replace—farmer judgment and local agricultural expertise.**

## 🛠️ Technologies Used

*   HTML5 / CSS3 / JavaScript (Vanilla)
*   NASA APIs (NASA POWER)
*   Charting libraries (Chart.js or similar)
*   GitHub Pages for deployment.
*   GitHub Pages para el despliegue.# maizeshift-jalisco
Climate dashboard for maize growers in Jalisco using NASA data.
