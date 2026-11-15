# 🌽 MaizeShift Jalisco

A decision-support tool to explore crop rotations in Jalisco, Mexico.
Developed by **Team Space Tapatíos** for the NASA Space Apps Challenge 2026 — Challenge: *Field Shift: Adapting Farms with NASA Data*.

👉 [Click here to test the live application (GitHub Pages)](https://spacetapatios.github.io/maizeshift-jalisco/)

## 📖 Overview

Farmers in Jalisco face shifting temperatures, unpredictable rainfall patterns, and water shortages. MaizeShift combines NASA climate and soil-wetness data with the farmer's priorities to compare crop rotation options that can strengthen soil health and help farms adapt to changing conditions.

## 🚀 Key Features

* **Historical Climate Analysis:** Uses NASA POWER data (1995–2025) to show trends in temperature, precipitation, extreme heat days and root-zone soil wetness.
* **Rotation Explorer:** Lets the farmer select soil type, irrigation level and priorities (water security, soil health, income, stability, low input cost) and compares different rotation strategies, including the existing one.
* **Interactive Map:** Displays maize regions in Jalisco to contextualize the data.
* **Data Download:** Export the data as CSV for further analysis.
* **Bilingual Interface (EN/ES):** Simple language designed for users with limited technical or geospatial experience.

## 🔬 Methodology & Data

* **Data Source:** NASA POWER (AG community): 2 m air temperature (T2M), bias-corrected precipitation (PRECTOTCORR), root-zone soil wetness (GWETROOT) and daily maximum temperature (T2M_MAX).
* **Processing:** Data is fetched live for each region's coordinates. The growing season is defined as June–October. Earlier period = 1995–2009, recent period = 2010–2025.
* **Model:** The rotation explorer calculates water supply (season rain + usable soil water + irrigation) and heat pressure to evaluate crops. Scores are weighted by the farmer's priorities.
* **Maps:** Current conditions in map popups come from Open-Meteo (not NASA data). Satellite imagery and place names are from Esri.

## ⚠️ Limitations & Transparency

* This tool is not a yield forecast. It provides signals to support decisions, to be combined with local agronomic advice.
* Crop and soil values are simplified, illustrative assumptions (typical ranges); they are meant to be replaced with local data and agronomist input.
* Uses one grid point per region (cells of about 0.5° × 0.625°); no yield or irrigation data is included. Soil wetness is model-based.
* The tool is designed to support, not replace, farmer judgment and local agricultural expertise.
* **Next steps:** NASA SMAP observations and MODIS/Landsat vegetation indices.

## 🛠️ Technologies Used

* HTML5 / CSS3 / JavaScript (vanilla)
* NASA POWER API
* [Chart.js / Leaflet: write the exact libraries you used]
* Open-Meteo API and Esri basemaps (non-NASA)
* GitHub Pages for deployment

## 🤖 Use of Super Intelligence (SI) Tools

In accordance with the NASA Space Apps Challenge guidelines, we disclose that this project was developed with the assistance of an AI chatbot (**Claude, by Anthropic**). SI tools were used for: [adjust to what applies: code development and debugging, text drafting, documentation, translation]. All content was reviewed by the team. No NASA logos, branding or design elements were used or modified.

## 👥 Team

Team Space Tapatíos — NASA Space Apps Challenge 2026
