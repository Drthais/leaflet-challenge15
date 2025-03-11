# leaflet-challenge15
# Earthquake Visualization Project

## Background

This project visualizes earthquake data from the United States Geological Survey (USGS) to provide a clear and interactive representation of seismic activity. The USGS collects extensive earthquake data, and this visualization aims to make that data more accessible and informative to the public and other organizations.

## Project Goal

To create a Leaflet map that displays earthquake data, reflecting magnitude and depth, with interactive popups and a legend. Optionally, to overlay tectonic plate data and provide layer controls.

## Data Sources

* **Earthquake Data:** USGS GeoJSON Feed (e.g., "All Earthquakes from the Past 7 Days").
    * Accessed via the JSON URL provided by the USGS.
* **Tectonic Plates Data (Optional):** [https://github.com/fraxen/tectonicplates](https://github.com/fraxen/tectonicplates)

## Project Structure

* `index.html`: Contains the HTML structure for the map.
* `logic.js`: Contains the JavaScript code for fetching, processing, and visualizing the data using Leaflet.
* `style.css`: contains the css styling for the html.

## Part 1: Earthquake Visualization

### Steps

1.  **Data Acquisition:**
    * Obtain the earthquake data from the USGS GeoJSON Feed.
    * Copy the URL of the desired dataset (e.g., "All Earthquakes from the Past 7 Days").
2.  **Map Creation:**
    * Use Leaflet to create a map centered on a relevant location.
    * Fetch the earthquake data using the provided URL.
3.  **Data Visualization:**
    * Plot each earthquake as a circle marker on the map using its longitude and latitude.
    * Set the marker size based on the earthquake's magnitude.
    * Set the marker color based on the earthquake's depth (deeper earthquakes are darker).
    * Add popups to each marker displaying earthquake details (magnitude, location, time, depth).
4.  **Legend Creation:**
    * Create a legend to explain the meaning of the marker size and color.

## Part 2: Optional Enhancements

### Steps

1.  **Tectonic Plates Overlay:**
    * Fetch tectonic plates data from the provided GitHub repository.
    * Plot the tectonic plate boundaries on the map.
2.  **Base Map Selection:**
    * Add multiple base map options for the user to select from.
3.  **Layer Controls:**
    * Implement layer controls to allow users to toggle the earthquake and tectonic plates layers on and off.

## How to Run

1.  Open `index.html` in a web browser.
2.  Interact with the map to explore the earthquake data.
3.  (Optional) Use the layer controls to toggle tectonic plates and base maps.

## Notes

* Ensure that Leaflet and any necessary dependencies are included in the project.
* The data is live, and will update according to the USGS data feed.
* The optional portion of the project requires an internet connection to load the tectonic plates geoJSON.
