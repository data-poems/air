# AIR

[![Live Site](https://img.shields.io/badge/live-dr.eamer.dev-00ffaa)](https://dr.eamer.dev/datavis/poems/air/)
[![MIT License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

Real-time air quality map for the world's 100 largest cities. Updates every 30 seconds with fresh AQI data from Open-Meteo. Click any city for detailed pollutant breakdowns (PM2.5, PM10, ozone, nitrogen dioxide).

## Features

- **Live data**: Open-Meteo Air Quality API
- **100 largest cities**: Global coverage from Beijing to Sao Paulo
- **Real-time updates**: Fresh data every 30 seconds
- **Interactive map**: Pan, zoom, click for details
- **Color coding**:
  - Green (0-50): Good
  - Yellow (51-100): Moderate
  - Orange (101-150): Unhealthy for sensitive groups
  - Red (151-200): Unhealthy
  - Purple (201+): Very unhealthy

## Technical Stack

- **Vanilla JavaScript**: No frameworks
- **Canvas API**: Hardware-accelerated rendering
- **Open-Meteo API**: Real-time AQI data
- **D3.js**: Geographic projections

## Files

- `index.html` - Main visualization
- `air_bubbles.html` - Alternate bubble view
- `hive/` - Production variant
- `dev/` - 5 experimental variants (attractor, globe, hive, minimalist)
- `social-card.jpg` - Open Graph image

## Local Development

```bash
python3 -m http.server 8000
# Visit http://localhost:8000
```

## Data Source

Open-Meteo Air Quality API
https://open-meteo.com/en/docs/air-quality-api

## Author

Luke Steuber — [dr.eamer.dev](https://dr.eamer.dev) — [@lukesteuber.com](https://bsky.app/profile/lukesteuber.com)

## License

MIT
