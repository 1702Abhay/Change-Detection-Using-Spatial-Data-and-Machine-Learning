# Change-Detection-Using-Spatial-Data-and-Machine-Learning
Monitored LULC changes using QGIS and supervised ML classifiers.

In this project, I performed Land Use Land Cover (LULC) change detection using multi-temporal satellite imagery. I used QGIS and Erdas imagine for preprocessing and visualization, and applied supervised machine learning classifiers to classify land cover for different years.

First, I collected satellite data (like Sentinel-2), performed preprocessing such as clipping, cloud masking, and band stacking. Then I created training samples for classes like vegetation, water, and built-up areas.

Using these samples, I trained a classifier (Random Forest) to generate LULC maps for each year. Finally, I performed post-classification comparison to detect changes over time and quantified transitions like vegetation to urban expansion.

This helped in understanding urban growth patterns and environmental changes.

# Workflow (Step-by-Step)
Step 1: Data Collection
Sentinel-2 imagery (different years)
AOI shapefile
Step 2: Preprocessing (QGIS)
Clip raster to AOI
Band stacking
Remove clouds (if needed)
Step 3: Training Data
Create polygons for:
Water
Vegetation
Built-up
Bare soil
Step 4: Classification
Use Random Forest / SVM
Step 5: Change Detection
Compare classified maps (Year1 vs Year2)
