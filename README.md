# FHIR Synthetic Dataset Analysis Notebook

## Overview
This Jupyter notebook provides an end-to-end analysis of a synthetic FHIR (Fast Healthcare Interoperability Resources) dataset. It demonstrates data loading, cleaning, transformation, and visualization for healthcare data conforming to the FHIR standard. The dataset is based on synthetic patient records from [SMART on FHIR's sample bulk datasets](https://github.com/smart-on-fhir/sample-bulk-fhir-datasets).

## Dataset Details
- **Source**: [SMART on FHIR Sample Bulk Datasets](https://github.com/smart-on-fhir/sample-bulk-fhir-datasets) (1000-patient synthetic dataset)
- **Resources Included**:
  - Patients
  - Conditions
  - Observations
  - Encounters
  - Immunizations
  - MedicationRequests
  - Procedures
  - DiagnosticReports

## Features
- **Data Processing**:
  - Loads NDJSON files for multiple FHIR resources
  - Extracts and normalizes nested FHIR fields (e.g., patient demographics, addresses, language preferences)
  - Merges clinical data across resources
- **Key Analyses**:
  - Condition prevalence statistics
  - Comorbidity analysis
  - Patient demographic distributions
  - Temporal trends in observations and diagnostics
- **Visualization**:
  - Interactive plots using Plotly
  - Geographical mapping of patient locations
  - Temporal analysis of medical events

## Requirements
- Python 3.7+
- Jupyter Notebook
- Dependencies:
  ```bash
  pandas numpy requests plotly matplotlib seaborn
Installation
Clone this repository

Install dependencies:

bash
pip install -r requirements.txt
Download the dataset from SMART on FHIR's repository and place the sample-bulk-fhir-datasets-1000-patients folder in your working directory.

Usage
Launch Jupyter Notebook:

bash
jupyter notebook
Open FHIR_synthetic_dataset_test.ipynb

Run cells sequentially to:

Load and preprocess data

Explore patient demographics

Analyze clinical conditions and observations

Generate interactive visualizations

Key Outputs
Patient demographic summaries

Top 10 prevalent medical conditions

Comorbidity network analysis

Temporal patterns in lab results and diagnostics

Geographical distribution of patients

Acknowledgements
Dataset provided by the SMART on FHIR team under the CC0 1.0 Universal License.

License
This notebook is shared under MIT License. Ensure proper attribution when reusing or modifying.
