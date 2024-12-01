# edar-xedar-expression-analysis
R scripts for analyzing Edar and Xedar gene expression data in mouse and rat tail development
# Gene Expression Analysis Scripts

This repository contains R scripts for analyzing gene expression data from the study "Differential Expression of Edar and Xedar During Mouse and Rat Tail Appendage Development".

## Overview

The scripts perform statistical analyses of Edar and Xedar gene expression data, including:
- Data quality control and normalization
- Two-way ANOVA with post-hoc tests
- Correlation analysis
- Polynomial regression modeling
- Data visualization

## Requirements

The following R packages are required:
- stats
- ggplot2
- car
- nlme

##Install using:
```R
"install.packages(c("stats", "ggplot2", "car", "nlme"))"

##Input Data Format
The scripts expect a CSV file named "edar_xedar_expression.csv" with the following columns:

day: developmental day (numeric)
species: mouse or rat (factor)
edar: Edar expression value (numeric)
xedar: Xedar expression value (numeric)
actin: β-actin expression value (numeric)

##Example
day,species,edar,xedar,actin
11,mouse,55.81,1176.26,1.02
12,rat,90.44,1833.53,0.98

##Usage
Place your data file in the working directory
Run the analysis:
source("expression_analysis.R")

##Output
The script generates:

Statistical test results (saved in analysis_results.RData)
Expression pattern plots (saved as PDF)
R-squared values for polynomial models
ANOVA results and correlation coefficients

##Citation
If you use these scripts, please cite:
Wisniewski SA (2024) Differential Expression of Edar and Xedar During Mouse and Rat Tail Appendage Development

##Contact
For questions or issues, please contact:
sa.wisniewski@sci4biz.edu.pl

##License
This code is available under the CC-BY 4.0 license.
