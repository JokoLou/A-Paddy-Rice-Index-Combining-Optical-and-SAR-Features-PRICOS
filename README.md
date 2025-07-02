# A-Paddy-Rice-Index-Combining-Optical-and-SAR-Features-PRICOS

This project provides code for calculating the Paddy Rice Index (PRICOS) by integrating optical and SAR time-series features. It supports both JavaScript and Python to accommodate users from different backgrounds.

---
## Data Requirements

The algorithm requires five satellite image time series as inputs:

1. Sentinel-2 NDVI during the paddy rice transplanting stage  
2. Sentinel-2 NDVI from tillering to maturity stages  
3. Sentinel-2 MNDWI during the transplanting stage  
4. Sentinel-1 VH during the transplanting stage  
5. Sentinel-1 VH from tillering to maturity stages  

All satellite data are open-access via Google Earth Engine (GEE).

---
## Usage

Please read the instructions before using the code.  

1. Clone this repository.  
2. Prepare your GEE credentials (for Python) or open the JavaScript notebook in GEE.  
3. Replace the sample paths with your own asset IDs.  
4. Run the script and inspect outputs in the console or export maps to your assets.

---

## Phenological Stages

Paddy rice growth stages can be determined using:

- A small number of ground-truth sample points  
- Existing regional cropping calendars  

---

## Citation

If you use PRICOS in your research, please cite: Lou, Y., Yang, G., Sun, W., Huang, K., Huang, J., Wang, L., & Liu, W. (2025).PRICOS: A Robust Paddy Rice Index Combining Optical and Synthetic Aperture Radar Features for Improved Mapping Efficiency.Remote Remote Sensing, 17(692). https://doi.org/10.3390/rs17040692
