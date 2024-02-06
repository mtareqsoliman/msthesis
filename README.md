# Project Overview:

This project is a part of a study that explores the application of machine learning techniques in developing seismic fragility models for structures with multiple interdependent failure modes. Our research explores the benefits and limitations of machine learning algorithms when used as an alternative approach to traditional time history analysis in developing fragility models.

## Motivation:
The motivation behind this project stemmed from the need to address the limitations of existing fragility curve development methods in the literature, particularly in capturing the complex relationships between multiple failure mechanisms. [(Liel et al. 2009)](https://doi.org/10.1016/j.strusafe.2008.06.002) introduced fragility curve development incorporating structural and record-to-record uncertainties, our study aims to enhance the accuracy and efficiency of fragility modeling through machine learning.

## Methodology:
A case study featuring a structure with a relatively shorter column subjected to seismic loading [(Pinto 2004)]( https://books.google.com.eg/books/about/Seismic_reliability_analysis_of_structur.html?id=TPAeAQAAIAAJ&redir_esc=y). The structure exhibits three primary failure mechanisms: flexural failure at the top and bottom sections, and shear failure; all of them occurs at the shorter column. Our methodology involved constructing a benchmark model by performing incremental dynamic analysis with extensive nonlinear time history analysis using 12 ground motion records; each scaled at different intensity measure levels; resulting in a large dataset of training data approximately 12,000 rows.

## Results:
Our findings revealed the limitations of traditional polynomial equations in capturing nonlinear relationships between failure mechanisms. However, artificial neural networks (ANN) demonstrated superior performance in developing median fragility models compared to the Response Surface Methodology (RSM) with Central Composite Design (CCD). Furthermore, The study observed a specific transition zone between controlling failure mechanisms, suggesting potential areas for optimization in future analyses.

## Reference:
Soliman, M.T.M. (2023). Application of machine learning algorithms in seismic fragility analysis of structures. Masters Thesis, Istanbul Technical University, Türkiye.
