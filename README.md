# ExtremeProjections

Exploring meteorological projections from Global Climate Models (GCMs) over **North America**, with a focus on extreme climate events in **Canada**.

---

## Description
Analyzing and visualizing meteorological projections from GCMs over North America, focusing on ecoregions, watersheds, and climate extremes. The project evaluates future climate variables, seasonal and annual trends, climate indices, and model uncertainties using a multi-model ensemble approach.

---

## Data Sources

### 1. Climate Projections: NEX-GDDP-CMIP6
[NASA Earth Exchange Global Daily Downscaled Projections (NEX-GDDP-CMIP6)](https://www.nccs.nasa.gov/services/data-collections/land-based-products/nex-gddp-cmip6)

Provides global, high-resolution daily climate projections from CMIP6 models.

**Key details:**  
- **Coverage:** 180°W–180°E, 60°S–90°N  
- **Resolution:** 0.25° × 0.25°  
- **Temporal range:** Daily from 1950-01-01 to 2100-12-31  
- **Variables include:**  
  - `tas` – Daily near-surface air temperature (K)  
  - `tasmax` / `tasmin` – Daily max/min near-surface air temperature (K)  
  - `pr` – Daily precipitation (kg m⁻² s⁻¹)  
  - `hurs` – Near-surface relative humidity (%)  
  - `huss` – Near-surface specific humidity (kg/kg)  
  - `rsds` / `rlds` – Surface shortwave/longwave radiation (W m⁻²)  
  - `sfcWind` – Near-surface wind speed (m s⁻¹)

### 2. Ecoregions
[Level III EPA ecoregions across North America](https://www.epa.gov/eco-research/ecoregions-north-america)

- Ecologically distinct areas based on climate, soil, vegetation, landform, and other factors.  
- Level III includes ~200 regions, suitable for analysis across North America.  

### 3. Watersheds
[Canadian Lake and River Hydrofabric (CLRH)](https://hydrology.uwaterloo.ca/CLRH/Hydrofabric.html)

- Provides polygons for watershed delineation

---

## Project Workflow

### 1. Ecoregion-level Analysis
- Compute future climate projections for each ecoregion and compare seasonal and annual trends across 21 GCMs.  
- Assess projections for **near-term (2025–2050), mid-term (2050–2075), and long-term (2075–2100)** periods and analyze changes relative to historical hindcasts (~25-year baseline, 1990–2015).  
- Depict model uncertainty.

### 2. Watershed-level Analysis
- Select specific basins in **Canada** for detailed future projection analysis.  
- Depict model predictions of variables over the **historical and future periods (1950–2100)**.  
- Depict model uncertainty.

### 3. Climate Indices & Extremes
- Calculate indices such as **Warm Spell, CDDM, TRC** and other metrics related to extreme events for the selected watersheds.  
- Analyze indices over **historical and future periods (1950–2100)**.  
- Assess model agreement in predicting extreme events.

---

## Usage
- Python scripts and notebooks handle data preprocessing, analysis, and visualization.  
- Example workflows demonstrate how to:  
  - Download and process NEX-GDDP-CMIP6 data  
  - Aggregate climate variables by ecoregion or watershed  
  - Calculate climate indices and visualize trends

---

## License
[........... e.g., MIT License]
