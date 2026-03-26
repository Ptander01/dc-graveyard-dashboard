# Data Center Graveyard Dashboard

A specialized visualization tool for tracking and analyzing at-risk, delayed, and blocked data center projects across the United States. This dashboard highlights community opposition factors, stage gate failures, and capacity at risk.

**Note:** This repository contains a sanitized version of the application. All proprietary data and real-world project specifics have been replaced with a synthetic dataset inspired by real-world patterns for demonstration purposes.

## Key Features

- **Interactive Status Map:** Built with MapLibre GL JS, featuring color-coded markers for blocked (red), delayed (orange), and withdrawn (gray) projects.
- **Opposition Analysis:** Filter projects by specific community opposition factors (Water, Electricity, Noise, Air Quality, Environment, etc.).
- **Stage Gate Tracking:** Analyze where projects fail in the development lifecycle (Zoning, Planning Commission, Environmental Review, etc.).
- **Data Table & Export:** Comprehensive data grid with CSV and GeoJSON export capabilities.
- **Analytics Charts:** ECharts-powered visualizations showing failure trends over time, stage exit analysis, and opposition category breakdowns.

## Tech Stack

### Frontend
- **Framework:** React 18 with TypeScript
- **Build Tool:** Vite
- **Styling:** Tailwind CSS (Neumorphic/Soft UI design)
- **Mapping:** MapLibre GL JS
- **Charts:** Apache ECharts (`echarts-for-react`)
- **Tables:** TanStack Table
- **Icons:** Lucide React

*Note: This dashboard runs entirely client-side using static JSON/GeoJSON data, requiring no backend server.*

## Getting Started

### Prerequisites
- Node.js (v18+)
- pnpm

### Start the Dashboard

Navigate to the frontend directory, install dependencies, and start the Vite development server:

```bash
cd frontend
pnpm install
pnpm dev
```

The dashboard will be available at `http://localhost:5174` (or `5173` depending on port availability).

## Data Architecture

The application relies on static synthetic data files located in `frontend/public/data/`:

- `projects.geojson`: Core project data with coordinates and status.
- `lookups.json`: Filter dropdown options and metadata.
- `statistics.json`: Pre-calculated KPI metrics (Capacity at risk, investment at risk, etc.).

## Portfolio Context

This project demonstrates expertise in specialized UI/UX design (neumorphism), client-side data filtering and aggregation, and translating complex socio-political data (community opposition) into actionable infrastructure intelligence.
