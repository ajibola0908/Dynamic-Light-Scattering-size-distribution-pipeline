# Dynamic-Light-Scattering-size-distribution-pipeline
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/)

A comprehensive Python pipeline for processing Dynamic Light Scattering (DLS) data from Malvern Zetasizer instruments. This tool automates the analysis of nanoparticle size distributions across different processing conditions, with adaptive peak detection, statistical analysis, and publication-quality visualization.

## Features
- **Automated Data Processing**: Parses Zetasizer export files and organizes measurements by pass type
- **Intelligent Filtering**: Automatically removes low-intensity artifacts
- **Adaptive Peak Detection**: Detects multiple peaks using scipy.signal.find_peaks with sample-specific optimization
- **Smart Configuration**: Auto-adjusts parameters for different materials (PBAT, PS, etc.)
- **Statistical Analysis**: Performs ANOVA and Tukey HSD tests
- **Publication-Quality Plots**: Professional visualizations with customizable styling
- **Batch Processing**: Analyze multiple samples simultaneously
- **Export Functions**: Saves processed data and peak tables to CSV

## Requirements
- Python 3.7+
- pandas
- numpy
- matplotlib
- scipy
- statsmodels
- openpyxl (optional, for Excel export)

## Installation
```bash
# Clone the repository
git clone https://github.com/ajibola0908/Dynamic-Light-Scattering-size-distribution-pipeline.git
cd dlsight

# Install dependencies
pip install -r requirements.txt
