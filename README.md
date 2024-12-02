# Georeferencing Script

This repository contains a script and methodology for performing automatic georeferencing of point cloud data using various filtering and transformation techniques.

## Introduction
The georeferencing process involves identifying and aligning point cloud data with a defined coordinate system. This project incorporates advanced clustering and transformation techniques, ensuring accurate georeferencing by utilizing centroid calculation, distance measurement, and angle verification for identifying prisms.

## Features
- Processing and filtering LAS files.
- DBSCAN clustering to identify point cloud patterns.
- Multi-stage filtering for identifying prisms based on:
  - Distance
  - Tolerance thresholds
  - Angular deviations
- Rigid transformation for aligning point clouds.
- Comprehensive transformation matrix application to the entire dataset.

## Dependencies
To use the scripts, install the following Python libraries:
- `numpy`
- `pandas`
- `scikit-learn`
- `laspy`
- `matplotlib`


