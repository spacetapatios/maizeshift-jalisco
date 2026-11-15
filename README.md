# 🌽 MaizeShift México (Jalisco)

A decision-support tool to explore crop rotations for maize growers in Jalisco and other regions of Mexico.
Developed by **Team Space Tapatíos** for the NASA Space Apps Challenge 2026 — Challenge: *Field Shift: Adapting Farms with NASA Data*.

👉 [Click here to test the live application (GitHub Pages)](https://spacetapatios.github.io/maizeshift-jalisco/)

## 📖 Overview

Farmers in Mexico face shifting temperatures, unpredictable rainfall patterns, and water shortages. MaizeShift combines NASA climate, soil-wetness, vegetation and terrain data with the farmer's priorities to compare crop rotation options that can strengthen soil health and help farms adapt to changing conditions.

## 🚀 Key Features

* **Historical Climate Analysis:** Uses NASA POWER data (1995–2025) to show trends in temperature, precipitation, extreme heat days and root-zone soil wetness.
* **Rotation Explorer:** Lets the farmer select soil type, irrigation level and priorities (water security, soil health, income, stability, low input cost) and compares rotation strategies, including the farmer's current rotation.
* **Scenario Sliders:** Test how changes in rainfall and extra warming affect the rotation ranking.
* **Vegetation Cover (MODIS NDVI):** Shows seasonal vegetation cover and possible bare-soil periods.
* **Rainfall Cross-Check:** Compares NASA POWER rainfall with an independent satellite source (GPM IMERG) to flag uncertainty.
* **Terrain and Erosion Risk (SRTM):** Estimates elevation and slope around each point.
* **Interactive Map:** 38 maize regions across Mexico, plus the option to click any point inside Mexico to analyze it. Includes a NASA GIBS NDVI map layer.
* **Glossary and Uncertainty Notes:** Plain-language explanations for non-expert users.
* **Data Download:** Export the data as CSV for further analysis.
* **Bilingual Interface (EN/ES).**

## 🔬 Methodology & Data

* **NASA POWER (AG community):** 2 m air temperature (T2M), bias-corrected precipitation (PRECTOTCORR), root-zone soil wetness (GWETROOT) and daily maximum temperature (T2M_MAX), fetched live for each region's coordinates (1995–2025).
* **NASA MODIS NDVI (MOD13Q1)** via the ORNL DAAC web service, **NASA GIBS** (NDVI map layer), **NASA GPM IMERG** (via NASA POWER, rainfall cross-check) and **NASA SRTM** (terrain and slope, via OpenTopoData).
* **Processing:** The growing season is defined as June–October. Earlier period = 1995–2009, recent period = 2010–2025. Trends use least-squares regression. A "dry season" has rainfall below 85% of the 1995–2025 average.
* **Model:** The rotation explorer calculates water supply (70% of season rain + usable soil water + irrigation) and heat pressure to evaluate crops. Scores are weighted by the farmer's priorities.
* **Non-NASA sources:** Current conditions in map popups come from Open-Meteo. Satellite imagery and place names are from Esri. If IMERG is unavailable, ERA5 (ECMWF) is used as the comparison source, and the app says so.

## ⚠️ Limitations & Transparency

* This tool is not a yield forecast. It provides signals to support decisions, to be combined with local agronomic advice.
* Crop and soil values are simplified, illustrative assumptions (typical ranges); they are meant to be replaced with local data and agronomist input.
* Uses one grid point per region (cells of about 0.5° × 0.625°); no yield, price, pest or irrigation data is included. Soil wetness is model-based.
* NDVI values are from a 250 m pixel at the region center, not a specific field.
* The tool is designed to support, not replace, farmer judgment and local agricultural expertise.
* **Next steps:** NASA SMAP observations, Landsat vegetation indices and local validation with farmers and agronomists.

## 🛠️ Technologies Used

* HTML5 / CSS3 / JavaScript (vanilla)
* Leaflet 1.9.4 (interactive map) and Chart.js 4.4.1 (charts)
* NASA APIs and data: POWER, MODIS (ORNL DAAC), GIBS, GPM IMERG, SRTM
* Open-Meteo API and Esri basemaps (non-NASA)
* GitHub Pages for deployment

## 🤖 Use of Super Intelligence (SI) Tools

In accordance with the NASA Space Apps Challenge guidelines, we disclose that this project was developed with the assistance of an AI chatbot (**Claude, by Anthropic**). SI tools were used for code development and debugging, text drafting, and translation. All content was reviewed by the team. No NASA logos, branding or design elements were used or modified.
<footer data-es='Equipo Space Tapatíos · NASA Space Apps Challenge 2026 · Field Shift: Adapting Farms with NASA Data<br>Desarrollado con asistencia de Claude (Anthropic), una herramienta de SI.' style="max-width:1100px;margin:auto;padding:0 20px 28px">Team Space Tapatíos · 2026 NASA Space Apps Challenge · Field Shift: Adapting Farms with NASA Data<br>Developed with assistance from Claude (Anthropic), an SI tool.</footer>

## 👥 Team

Team Space Tapatíos — NASA Space Apps Challenge 2026
