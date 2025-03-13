Route Optimization with OpenRouteService

# Overview

This project contains five Jupyter notebooks in the folder serviceroute that utilize the OpenRouteService API to optimize and visualize travel routes. The primary goal is to calculate efficient travel paths for a set of locations while considering constraints such as travel time, vehicle type, and required personnel. The generated routes are displayed on interactive maps using Folium.

## Features

Route Calculation: Computes optimal travel routes based on predefined coordinates.

Travel Time Estimation: Uses OpenRouteService to determine the travel time between locations.

Vehicle & Personnel Constraints: Ensures routes adhere to specific vehicle and personnel requirements.

Daily Route Splitting: Accounts for mandatory rest periods when the total travel time exceeds 8 hours.

JSON Data Integration: Reads coordinates and contract information from external JSON files.

Visualization: Uses Folium to display routes on an interactive map.

## Requirements

To run these notebooks, install the required dependencies using:

pip install openrouteservice folium

Additionally, ensure you have an OpenRouteService instance running locally or an API key for remote access.

## Usage

Place your coordinate data in a JSON file (e.g., hkauto2karte.json or test1.json).

Update the notebooks to reference the correct JSON file.

Run the notebooks to generate optimized routes and visualize them on a map.

## Files

Notebook 1: Loads JSON coordinate data and visualizes routes using Folium.

Notebook 2: Computes optimal travel paths considering vehicle and personnel constraints.

Notebook 3: Splits routes into daily segments to ensure compliance with driving hour regulations.

Notebook 4: Incorporates return travel time and further optimizes route calculations.

## Notes

Ensure OpenRouteService is properly configured before running the notebooks.

If using a remote API, replace base_url='http://localhost:8080/ors' with a valid API key.

## Future Improvements

Enhance optimization algorithms for better efficiency.

Integrate real-time traffic data for more accurate travel time estimation.

Extend visualization features with additional map layers and route details.

