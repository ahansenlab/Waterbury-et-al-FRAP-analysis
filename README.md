[![DOI](https://zenodo.org/badge/643759002.svg)](https://zenodo.org/doi/10.5281/zenodo.11089013)

# Waterbury-et-al-FRAP-analysis
This repository contains the fluorescence recovery after photobleaching (FRAP) analysis code used to analyze the data in the manuscript "Dynamic Masking by a Disordered Region Controls LSD1 Enhancer Silencing" by Waterbury et al. The code provided here in a python jupyter notebook format performs the following basic functions:
- reads and aggregates csv files containing bleaching data after drift correction with these columns: time, intensity, intensity_raw, nonbleach, corrected_nonbleach, nuclear_radius, roi_radius, gap_ratio, bleaching_depth, radius_uniform, bleach_distances, bleach_profile
- visualizes the raw data from these files
- plots radial intensity profiles and quality control metrics for the datasets provided if available
- fits one and two state binding models to the data and plots with 95% confidence intervals
- visualizes the comparison between multiple conditions
- performs a bootstrapping routine on the FRAP curves to assess significance between fitted parameters

## Installation:
1. Clone the repository:
```
    git clone https://github.com/DomenicN/Waterbury-et-al-FRAP-analysis.git
```

2. Ensure `conda` and `jupyter` are available and type in the terminal.

```
    jupyter notebook
```
Navigate to the notebook "FRAP_Analysis.ipynb" and open it.

3. Ensure the following packages are installed in the kernel
- numpy
- matplotlib
- pandas
- seaborn
- scipy
