# ShoreLIM
shoreLIM is a easy Python tool designed to run in GoogleColab for extracting annual shorelines from composite satellite imagery acquired by Landsat 5, 7, 8, and 9. 
The tool processes imagery over a user-defined area of interest (AOI), supports shoreline delineation using commonly used spectral indices, and applies the marching squares algorithm to achieve sub-pixel shoreline positioning.
```mermaid
flowchart TD
    A[Input polygons - AOI] --> B[Landsat imagery]
    B --> C[Cloud masking and annual composites]
    C --> D[MNDWI calculation]
    D --> E[Otsu thresholding]
    E --> F[Shoreline extraction]
    F --> G[Export GeoJSON]
```
