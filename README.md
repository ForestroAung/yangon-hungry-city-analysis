# The Hungry City: Yangon Food Scene Analysis

An end-to-end data science project analyzing the culinary landscape of Yangon, Myanmar, using OpenStreetMap (OSM) data and geospatial visualization.

##  Project Overview
This project identifies restaurant density, "food deserts," and cuisine distribution across Yangon. By extracting data from the Overpass API, the analysis reveals which townships are culinary hotspots and where infrastructure for food services is lacking.

##  Key Features
* **Automated Data Extraction:** Uses OpenStreetMap's Overpass API to fetch real-time geospatial data for 1,200+ establishments.
* **Geospatial Visualization:** An interactive Folium Heatmap showing restaurant density clusters.
* **Data Cleaning & Imputation:** Addressed a 90% missing-data rate in cuisine tags by using `amenity` types to categorize "Unknown" entries into "General Dining," "Cafe & Bakery," and "Quick Service."
* **Deduplication:** A custom spatial-deduplication logic to ensure unique entries based on name and coordinate proximity.

## Tech Stack
* **Language:** Python
* **Data Libraries:** Pandas, Requests (Overpass API)
* **Visualization:** Folium (Leaflet.js), Matplotlib
* **Environment:** Google Colab / Jupyter Notebooks

## Key Insights
* **Hotspots:** Downtown (Sule/Latha) and Bahan exhibit the highest restaurant density.
* **Food Deserts:** Significant gaps in food service infrastructure were identified in Dala and South Dagon.
* **Cuisine Trends:** While "General Dining" dominates, there is a rising trend of "Cafe & Bakery" establishments in Sanchaung and Hlaing townships.

##  Visualizations
<img width="1226" height="736" alt="image" src="https://github.com/user-attachments/assets/3bdc36d7-9eca-4da4-966f-f7b16d2a183d" />

<img width="495" height="292" alt="image" src="https://github.com/user-attachments/assets/92febd7c-99fe-4b35-870f-44fef1f0244a" />


## How to Run
1. Clone this repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Run the script: `python yangon_food_analysis.py`.
4. Open `yangon_food_heatmap.html` in your browser to view the interactive map.
