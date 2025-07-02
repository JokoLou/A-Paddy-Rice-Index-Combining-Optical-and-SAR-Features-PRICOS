# A Robust Paddy Rice Index Combining Optical and SAR Features — PRICOS

This project provides code for calculating the Paddy Rice Index (PRICOS), which integrates optical and synthetic aperture radar (SAR) time-series features. The method supports both JavaScript and Python implementations, making it accessible to users from various backgrounds.

---

## Data Requirements

The algorithm requires the following five satellite image time series as inputs (recommended variable names in parentheses):

1. Sentinel-2 NDVI during the paddy rice transplanting stage (`NDVI_FT`)  
2. Sentinel-2 NDVI from the tillering to maturity stages (`NDVI_TM`)  
3. Sentinel-2 MNDWI during the transplanting stage (`MNDWI_FT`)  
4. Sentinel-1 VH polarization during the transplanting stage (`VH_FT`)  
5. Sentinel-1 VH polarization from the tillering to maturity stages (`VH_TM`)
6. The difference in day-of-year (DOY) between the maximum VH polarization value during the tillering to maturity stages and the minimum VH polarization value during the transplanting stage, derived from Sentinel-1 data (`l`)

All input data can be processed and downloaded using Google Earth Engine (GEE).

---

## Usage Instructions

Please read the following notes carefully before using the code:

- A complete example script is provided for JavaScript users. The script can be run directly in the GEE Code Editor without any additional data preparation. (For large-scale applications, to improve computational efficiency, we recommend using a fixed value for the difference in day-of-year between VH maximum and minimum: 90 for plains, and 60 for mountainous regions.)  
- For Python users, please prepare the required datasets according to the "Data Requirements" section before running the script.

---

## Phenological Stage Definition

Paddy rice growth stages can be identified using:

- A small number of ground-truth samples  
- Regional crop calendars

---

## Citation

If you use the PRICOS method in your research, please cite:
Lou, Y., Yang, G., Sun, W., Huang, K., Huang, J., Wang, L., & Liu, W. (2025). PRICOS: A Robust Paddy Rice Index Combining Optical and Synthetic Aperture Radar Features for Improved Mapping Efficiency.Remote Sensing, 17(692). https://doi.org/10.3390/rs17040692
