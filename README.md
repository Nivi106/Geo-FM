# 🌍 Geo-FM: Multi-Temporal Flood Mapping Using Sentinel-2 NDWI Change Detection

## Overview

This project demonstrates an end-to-end geospatial data engineering workflow for flood extent mapping using Sentinel-2 satellite imagery.

The workflow includes metadata extraction, quality assessment, representative sampling, scalable raster processing using Xarray and Dask, cloud-ready storage using Zarr, GeoPrepBench benchmarking, flood detection using NDWI change detection, and visualization in QGIS.

## Project Workflow

Sentinel-2 Images
        │
        ▼
Metadata Extraction
        │
        ▼
Quality Assessment
        │
        ▼
Representative Sampling
        │
        ▼
Xarray Data Cube
        │
        ▼
Parallel Processing with Dask
        │
        ▼
Zarr Export
        │
        ▼
GeoPrepBench Validation
        │
        ▼
NDWI Change Detection
        │
        ▼
Flood Mask Generation
        │
        ▼
QGIS Visualization

## Technologies Used

- Python
- Google Earth Engine
- QGIS
- Rasterio
- Rioxarray
- Xarray
- Dask
- Zarr
- NumPy
- GeoPrepBench


## Repository Structure
Geo-FM/

├── config/
├── data/
│   ├── raw/
│   ├── metadata/
│   ├── curated/
│   └── benchmark/
│
├── src/
│   ├── metadata.py
│   ├── quality.py
│   ├── sampling.py
│   ├── datacube.py
│   ├── dask_pipeline.py
│   ├── zarr_export.py
│   ├── geoprepbench.py
│   └── flood_mapping.py
│
├── outputs/
├── screenshots/
├── README.md
└── requirements.txt

## Methodology

### 1. Metadata Extraction

Image metadata was extracted to organize the dataset and improve reproducibility.

### 2. Quality Assessment

Image quality was evaluated using cloud cover, geographic diversity, biome diversity, and temporal distribution.

### 3. Representative Sampling

A representative sampling strategy was designed to improve model generalization while reducing geographic bias.

### 4. Data Cube Generation

Raster imagery was converted into an Xarray Data Cube for scalable multidimensional analysis.

### 5. Parallel Computing

Dask was used for chunked and parallel raster processing.

### 6. Cloud-Optimized Storage

Processed data were exported in Zarr format for efficient storage and future machine learning workflows.

### 7. Dataset Benchmarking

GeoPrepBench was used to evaluate dataset readiness.

### 8. Flood Detection

Flood extent was mapped using multi-temporal NDWI change detection.

### 9. Visualization

The resulting flood mask was visualized using QGIS.

## Results

### Flood Extent Map
![Flood Map](screenshots/FloodMap.png)

## Skills Demonstrated

- Remote Sensing
- Geospatial Data Engineering
- Satellite Image Processing
- Data Cube Construction
- Parallel Computing
- Cloud-ready Raster Storage
- Flood Mapping
- GIS Visualization
- Python Development
- Reproducible Workflows

---

## Future Improvements

- Semantic segmentation using U-Net
- Foundation Models for Earth Observation
- Time-series flood monitoring
- Cloud Optimized GeoTIFF generation
- STAC integration
- Machine Learning-based flood classification

---

## Author

Nivedita Vee

Geospatial Data Science | Remote Sensing | GIS | Machine Learning