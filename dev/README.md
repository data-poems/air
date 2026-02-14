# Global Air Quality Bubbles

A data visualization poem that maps global air quality (AQI) to organic, floating bubbles.

## Overview
This project visualizes the invisible atmosphere we breathe. Using real-time data from the Open-Meteo API, it generates particles for major global cities. The number, speed, and color of the particles correspond to the Air Quality Index (US AQI).

- **Green**: Good air
- **Yellow/Orange**: Moderate/Sensitive
- **Red/Purple**: Unhealthy/Hazardous

## Data Source
**Open-Meteo Air Quality API**
- Endpoint: `https://air-quality-api.open-meteo.com/v1/air-quality`
- License: CC-BY 4.0 (Non-commercial use)
- Attribution: Data provided by Open-Meteo.com

## Technical Details
- **Batching**: Requests are batched to minimize API calls (50 cities per request).
- **Limits**: The implementation is designed to stay well under the Open-Meteo free tier limit (10,000 requests/day).
- **Rendering**: HTML5 Canvas with a custom particle system.

## Running Locally
No build step required. Simply serve the directory:
```bash
python3 -m http.server 8000
```
Then navigate to `http://localhost:8000/`.
