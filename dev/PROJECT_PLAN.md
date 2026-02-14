# Global Air Quality Bubbles - Project Plan

## Objective
Visualize real-time air quality data (AQI) from major cities worldwide using a floating bubble visualization. The project uses the Open-Meteo Air Quality API.

## Architecture
- **Frontend**: Single HTML file with Canvas API for particle rendering.
- **Data Source**: Open-Meteo Air Quality API (Free, non-commercial).
- **Style**: Minimalist, dark mode, neon accents.

## Current Status
- [x] Basic visualization loop.
- [x] Particle system linked to AQI values.
- [x] Responsive canvas.
- [x] Data fetching from Open-Meteo.
- [x] Optimization: Implemented request batching to support more cities.
- [x] Expanded city list to ~80 locations.

## Roadmap
- [ ] **Data**: Add more cities (aiming for 100+).
- [ ] **Features**:
    - [ ] Add search functionality.
    - [ ] Show detailed pollutants (PM2.5, PM10) on hover.
    - [ ] Add historical trend lines.
- [ ] **Performance**: Optimize particle count for low-end devices if city count grows > 200.
