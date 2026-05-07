---
layout: default
title: Soil Erosion Assessment in Aizawl
---

# Hybrid Machine Learning-RUSLE Approach for Soil Erosion Assessment

![Project overview image](../assets/images/<cover>.png)

## Overview

[cite_start]This study quantifies annual soil loss and delineates high-risk erosion zones in the Aizawl district of Mizoram, Northeast India[cite: 5, 6]. [cite_start]By integrating the Revised Universal Soil Loss Equation (RUSLE) with Machine Learning (ML), the project identifies a critical "erosion paradox" where high forest cover masks localized degradation hotspots caused by extreme topography[cite: 18, 19].

[cite_start]**Study Area:** Aizawl District, Mizoram, India [cite: 5]
[cite_start]**Duration:** October 2025 – March 2026 [cite: 592]
[cite_start]**Role:** Lead Researcher / Modeler [cite: 7, 573]
[cite_start]**Status:** Completed (Published in *Discover Soil*) [cite: 1, 592]

---

## Methods & Tools

**Data Sources**

- [cite_start]**Precipitation:** CHIRPS daily gridded rainfall data (2001–2024)[cite: 133].
- [cite_start]**Soil Properties:** USDA soil classification database (250m resolution)[cite: 166].
- [cite_start]**Topography:** SRTM Digital Elevation Model (30m resolution)[cite: 173].
- [cite_start]**Land Cover:** Sentinel-2 imagery and Dynamic World near real-time (NRT) data (10m resolution)[cite: 188, 194].

**Processing Steps**

1. [cite_start]**Factor Computation:** Calculated R, K, C, and P factors using parallelized pixel-based operations in Google Earth Engine (GEE)[cite: 17, 128].
2. [cite_start]**Terrain Analysis:** Computed the Slope Length and Steepness (LS) factor in ArcGIS 10.8 to maintain stability in rugged terrain[cite: 17, 128].
3. [cite_start]**Hybrid Modeling:** Integrated RUSLE parameters with Random Forest (RF) and Support Vector (SV) machine learning algorithms[cite: 16].
4. [cite_start]**Risk Zonation:** Performed a Weighted Index Overlay (WIO) to identify probability zones based on land use, slope, and rainfall[cite: 199, 201].

**Tools Used**

| Tool | Purpose |
|------|---------|
| **Google Earth Engine** | [cite_start]Parallel processing of high-resolution satellite and climate data [cite: 17, 92] |
| **ArcGIS 10.8** | [cite_start]LS factor computation and IDW interpolation [cite: 17, 158] |
| **Random Forest (RF)** | [cite_start]Predictive modeling with high accuracy ($R^{2}=0.93$) [cite: 18, 384] |
| **Sentinel-2** | [cite_start]NDVI generation for cover management (C factor) analysis [cite: 180] |

---

## Key Findings

- [cite_start]**Model Performance:** Random Forest significantly outperformed Support Vector models, achieving an $R^{2}$ of 0.93 against the RUSLE baseline[cite: 18, 384].
- [cite_start]**High Erosion Rates:** The estimated mean annual soil loss reached approximately **151.15 t/ha/yr**, primarily driven by extreme topographic relief (LS values up to 83)[cite: 18, 265].
- [cite_start]**The Erosion Paradox:** Over 45% of the district falls into moderate to very-high erosion-prone areas, specifically targeting barren lands and steep riverbanks despite overall high regional forest cover[cite: 19, 505].

---

## Links

[View Project PDF](../assets/Project.pdf){ .md-button }
[View Journal Publication](https://doi.org/10.1007/s44378-026-00191-3){ .md-button }
