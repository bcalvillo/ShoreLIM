# ShoreLIM
shoreLIM is a easy Python tool designed to run in GoogleColab for extracting annual shorelines from composite satellite imagery acquired by Landsat 5, 7, 8, and 9. 
The tool processes imagery over a user-defined area of interest (AOI), supports shoreline delineation using commonly used spectral indices, and applies the marching squares algorithm to achieve sub-pixel shoreline positioning.

flowchart TD
    A["Input polygons"]
    B["Landsat imagery"]
    C["Cloud masking"]
    D["Annual composites"]
    E["MNDWI"]
    F["Otsu threshold"]
    G["Shoreline extraction"]
    H["GeoJSON export"]

    A --> B --> C --> D --> E --> F --> G --> H
