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


## Workflows

1. **Read the LAS File**: Load the point cloud data from a `.las` file.
2. **Unit Conversion**: Ensure consistent units for further processing.
3. **Clustering with DBSCAN**: Identify clusters with specific intensity values.
4. **Centroid and Distance Calculation**: Calculate centroids and compare distances with actual prism data.
5. **Multi-Stage Filtering**:
   - **Distance-based Filtering**: Filter using different tolerances.
   - **Angle-based Filtering**: Eliminate "fake" prisms by comparing angular deviations.
6. **Rigid Transformation**: Perform georeferencing using transformation matrices.
7. **Apply Transformation**: Transform the entire point cloud data using the derived transformation matrix.

