# CLAUDE.md
<!-- Navigation: ~/html/datavis/poems/air/CLAUDE.md -->
<!-- Parent: ~/html/datavis/poems/CLAUDE.md -->
<!-- Map: ~/CLAUDE_MAP.md -->

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Real-time air quality visualization for the world's 100 largest cities using Open-Meteo Air Quality API. Multiple visual interpretations with an active dev workspace.

Live at: https://dr.eamer.dev/datavis/poems/air/

See `README.md` for feature details and data source.

## Structure

```
air/
├── index.html          # Main visualization — Canvas particle map with D3 geo
├── air_bubbles.html    # Alternate bubble view
├── hive/
│   └── index.html      # Production variant — constellation breathing pattern
├── dev/                # 5 experimental variants
│   ├── index.html      # Dev version of main
│   ├── attractor.html  # Mathematical attractor variant
│   ├── globe.html      # 3D globe variant
│   ├── hive.html       # Dev version of hive
│   ├── minimalist.html # Stripped-down variant
│   ├── world-110m.json # TopoJSON world boundaries
│   └── PROJECT_PLAN.md # Development roadmap
└── social-card.jpg     # OG image
```

## Technology

- **Canvas 2D** + **D3.js v7**: Geographic projections, particle rendering
- **Open-Meteo API**: Live AQI data, batched calls every 30 seconds
- **No frameworks**: Vanilla JavaScript

## Key Patterns

- AQI color scale: Green (0-50) → Yellow (51-100) → Orange (101-150) → Red (151-200) → Purple (201+)
- Live data refresh via `setInterval` with batched API requests to minimize calls
- Multiple render strategies across variants (particles, bubbles, constellation, globe)

## Parent Documentation

- `../CLAUDE.md` — Poems collection overview
- `../STYLE_GUIDE.md` — Full design system
