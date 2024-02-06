# Project Overview

This project is a part of a study that explores the application of machine learning techniques in developing seismic fragility models for structures with multiple interdependent failure modes. Our research explores the benefits and limitations of machine learning algorithms when used as an alternative approach to traditional time history analysis in developing fragility models.

# Motivation
The motivation behind this project stemmed from the need to address the limitations of existing fragility curve development methods in the literature, particularly in capturing the complex relationships between multiple failure mechanisms. (Liel et al. [2009](https://doi.org/10.1016/j.strusafe.2008.06.002)) introduced fragility curve development incorporating structural and record-to-record uncertainties, our study aims to enhance the accuracy and efficiency of fragility modeling through machine learning.

# Methodology
A case study featuring a structure with a relatively shorter column subjected to seismic loading (Pinto, [2004]( https://books.google.com.eg/books/about/Seismic_reliability_analysis_of_structur.html?id=TPAeAQAAIAAJ&redir_esc=y)). The structure exhibits three primary failure mechanisms: flexural failure at the top and bottom sections, and shear failure; all of them occurs at the shorter column. Our methodology involved constructing a benchmark model by performing incremental dynamic analysis with extensive nonlinear time history analysis using 12 ground motion records; each scaled at different intensity measure levels; resulting in a large dataset of training data approximately 12,000 rows.

## [1_OpenSeesAnalysis.ipynb](https://github.com/mtareqsoliman/msthesis/blob/main/1_OpenSeesAnalysis.ipynb)

### Overview
The file `1_OpenSeesAnalysis.ipynb` provides an in-depth exploration of the OpenSees analysis conducted in the context of the master's thesis. OpenSees is employed for nonlinear time history analysis to assess structural performance under seismic events.

### Key Sections
1. **Installing Required Libraries:** The notebook begins by ensuring OpenSees and other necessary libraries are installed.

2. **Defining the Structural Model:** The structure used for analysis is modeled using OpenSees. The the material properties, geometry, and loading conditions are defined.

3. **Performing Nonlinear Time History Analysis:** Nonlinear time history analyses are executed and repeated for each analysis case.

4. **Post-Processing and Visualization:** The obtained results are post-processed and visualized to gain insights into the structural response.

## [2_Results_of_MC_RSM_ANN_StdCase.ipynb](https://github.com/mtareqsoliman/msthesis/blob/main/2_Results_of_MC_RSM_ANN_StdCase.ipynb)

### Overview
The file `2_Results_of_MC_RSM_ANN_StdCase.ipynb` presents the results and analysis derived from employing various methods, which are: 1) Monte Carlo simulations (MC), 2) Response Surface Methodology (RSM), and 3) Artificial Neural Networks (ANN). This notebook is a follow-up to the OpenSees analysis, utilizing the results obtained to develop fragility models.

### Key Sections
1. **Developing the Benchmark Model:** The study introduces two sampling methods, Monte Carlo Simulations and Latin Hypercube Simulations, and focuses on the Monte Carlo approach. It includes the preparation of the training dataset, creating a pivot table, calculating fragility model parameters, estimating median fragility model parameters, and plotting relevant visualizations.

2. **Response Surface:** This section is about the application of Central Composite Design as a sampling method, the preparation of the training dataset, creating a pivot table, calculating fragility model parameters, and plotting response surfaces, residual errors, and RMSE for points.

3. **Artificial Neural Networks (ANN):** The study explores the utilization of ANN for predicting fragility model parameters. Sections cover preparing the training dataset, calculating fragility model parameters, training the ANN, developing the median ANN model, and plotting relevant visualizations.

Please refer to the respective notebooks for detailed code implementations, analysis procedures, and visualizations.


# Results
Our findings revealed the limitations of traditional polynomial equations in capturing nonlinear relationships between failure mechanisms. However, artificial neural networks (ANN) demonstrated superior performance in developing median fragility models compared to the Response Surface Methodology (RSM) with Central Composite Design (CCD). Furthermore, The study observed a specific transition zone between controlling failure mechanisms, suggesting potential areas for optimization in future analyses.

# Please see
Soliman, M.T.M. (2023). _Application of machine learning algorithms in seismic fragility analysis of structures_. Masters Thesis, Istanbul Technical University, [Türkiye](https://tez.yok.gov.tr).
