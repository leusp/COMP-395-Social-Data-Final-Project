# COMP-395-Social-Data-Final-Project
## Project Overview
This repository houses the code and analysis for the project, "A Socioeconomic Comparison of Housing Prices' Response to Eaton and Palisades Fires."

The project uses a Difference-in-Differences (DiD) quasi-experimental design to measure the immediate causal impact of the January 2025 Palisades and Eaton Wildfires on local housing markets, comparing the price resilience between two socioeconomically distinct communities:
- Treatment Group: Pacific Palisades (affluent, high-resource community).
- Comparison Group: Altadena (less affluent community, serving as the counterfactual).

The  analysis, based on aggregated Zillow data, resulted in a non-significant finding, underscoring the need for the advanced geospatial checks outlined in the future research section.


## Dependencies
To run the core analysis notebook (Social_Data_Sci_Midterm_Hackathon.ipynb), the following Python libraries are required:
```python
import numpy as np
import pandas as pd
import geopandas as gpd
import matplotlib.pyplot as plt
import seaborn as sns
import statsmodels.formula.api as smf
# Utility for downloading Google Drive files
!pip install gdown
```

## Data Sources & Acquisition
The analysis relies on public data sources, filtered to a 12-month event window (6 months before and 6 months after the fire event date of January 7, 2025).
- Zillow Home Value Index (ZHVI)
- ZIP Codes & Time
- CAL FIRE DINS Data & Perimeters
