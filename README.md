# S2-Coast-CA
Sentinel-2 Coastal Habitats of California Mapping Project
Authors: Christiana Ade (christiana.ade@jpl.nasa.gov) and Katie Osborn (kposborn@ucla.edu)

The scripts in this repository are used to build and apply a random forest classifier for classifying beach and rocky shore habitats along the California (CA) Coast. 

The 01_Build_Classifier script uses 1) pre-selected Sentinel-2 tiles (determined by best low-tide images from 2022) along the CA coast and 2) imported sets of class training points (based on habitat classifications the California Aquatic Resource Inventory (CARI) and adjusted as needed) to build a random forest classifier capable of classifying beaches, rocky shore, water, whitecaps, and vegetation along the CA coast. You can also use this script to visualize the resulting classification of the CA coast.

The 02_Export_Classification script imports the random forest classifier from the above script, applies the classification to the Sentinel-2 2022 CA coast mosaic, and exports the resulting classification in batches in raster and vector formats. You must run the 01_Build_Classifier script before running 02_Export_Classification.
