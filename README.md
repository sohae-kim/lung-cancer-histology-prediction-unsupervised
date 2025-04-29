# Lung Cancer Histology Prediction using RNA Sequencing Data

This repository contains the final project for CSCA 5632 Unsupervised Algorithms in Machine Learning at the University of Colorado Boulder MS-CS program.

## Project Overview

This project was inspired by the paper "[Deep Radiotranscriptomics of Non-Small Cell Lung Carcinoma for Assessing Molecular and Histology Subtypes with a Data-Driven Analysis](https://doi.org/10.3390/diagnostics11122383)" by E. Trivizakis *et al*. The paper developed and evaluated a "deep radiotranscriptomics" framework for non-small cell lung carcinoma (NSCLC) that combined two types of data: deep features extracted from CT images and transcriptomic (RNA) data.

## Background

Non-small cell lung cancer (NSCLC) is the most common type of lung cancer. The main types of NSCLC include adenocarcinoma, squamous cell carcinoma, and large cell lung cancer. While the original paper used deep learning to predict tumor histology (the cellular composition of the cancerous tumor), this project explores unsupervised learning approaches.

## Data Sources

This project uses data from the following sources:
- [RNA Sequence Data](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE103584)
- [Clinical Data](https://www.cancerimagingarchive.net/collection/nsclc-radiogenomics/)

## Project Objectives

The primary objective is to implement unsupervised learning algorithms to predict NSCLC histology (specifically distinguishing between adenocarcinoma and squamous cell carcinoma). This approach allows us to evaluate whether gene expression patterns naturally cluster according to histological subtypes without explicit labels.

## Project Structure

This notebook is organized into the following sections:

1. **Data Loading and Preprocessing**
    - Loading RNA sequencing and clinical data
    - Handling missing values
   
2. **Exploratory Data Analysis (EDA)**
    - Distribution of histological subtypes
    - Gene expression patterns across subtypes
    - Correlation analysis between key genes

3. **Dimension Reduction with PCA**
    - Normalization
    - Reducing high-dimensional gene expression data

4. **Unsupervised Learning & Visualization**
    - Methods implemented:
        - K-means clustering
        - Hierarchical clustering
        - Non-negative Matrix Factorization (NMF)
    - Evaluation of clustering performance against known histology labels
    - t-SNE plots of clusters vs. true histology
    - Comparison of clustering methods

6. **Discussion and Conclusions**
    - Performance comparison across methods

## Key Findings

The project demonstrates how unsupervised learning methods can identify patterns in gene expression data that correspond to different histological subtypes of lung cancer. The analysis shows that:

- Gene expression data contains sufficient information to distinguish between adenocarcinoma and squamous cell carcinoma.
- Different clustering methods exhibit different levels of success in capturing the underlying structure of the data.
- The results highlight the potential of unsupervised learning approaches as complementary tools for cancer subtype classification.

## Technologies Used

- Python
- pandas, numpy for data manipulation
- scikit-learn for machine learning algorithms
- matplotlib, seaborn for visualization
- Various metrics for cluster evaluation

## Repository Structure

- `final_final.ipynb`: Jupyter notebook containing all code and analysis
- `README.md`: Project overview and documentation
- Data files (not included in repository due to size constraints)

## Installation and Usage

1. Clone this repository
2. Install required dependencies: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`
3. Download the data from the sources mentioned above
4. Run the Jupyter notebook to replicate the analysis

## Acknowledgments

- University of Colorado Boulder MS-CS program
- The original research on deep radiotranscriptomics that inspired this project: "[Deep Radiotranscriptomics of Non-Small Cell Lung Carcinoma for Assessing Molecular and Histology Subtypes with a Data-Driven Analysis](https://doi.org/10.3390/diagnostics11122383)" by E. Trivizakis *et al*.

## Note

This notebook was uploaded to GitHub as required for the final project submission and evaluation in the CSCA 5632 course.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
