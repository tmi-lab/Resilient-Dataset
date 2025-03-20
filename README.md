## Resilient Dataset

- [Resilient Dataset](#description)
  * [Summary of Data](#summary-of-data-tables-and-recorded-variables)
  * [Running the code](#running-the-code)
  
# Description
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15045663.svg)]([https://doi.org/10.5281/zenodo.15045663]) 
<br/>

RESILIENT Dataset: A Multimodal Approach to Monitoring Ageing-Related Multi-Morbidities and Cognitive Decline.
The dataset is available on its corresponding [Zenodo repository](https://zenodo.org/record/15045663).
<!--The full description of this dataset is published in Nature Scientific Data: [paper](https://doi.org/10.1038/s41597-023-02519-y)-->

The dataset is provided for research purposes and supporting patient care. 

Please acknowledge the Surrey and Borders Partnership NHS Foundation Trust and Howz in any publication or use of this dataset. 


### Summary of Data Tables and Recorded Variables

| **Device**     | **Table Name**         | **Variables** |
|--------------|----------------------|------------------------------------------------------------------|
| **ScanWatch** | **Steps**            | - **Steps**: Number of steps recorded per hour. <br> - **Timestamp**: Timestamp of each record. |
|              | **Heart Rate**        | - **Heart Rate**: Measurements taken every 10 minutes. <br> - **Timestamp**: Timestamp of each record. |
| **Sleep Mat** | **Sleep States**      | - **Sleep State**: One of four sleep states (Light, Deep, REM, Wake up). <br> - **Start Timestamp**: Start time of the corresponding sleep state. <br> - **End Timestamp**: End time of the corresponding sleep state. |
|              | **Sleep Physiology**   | - **Heart Rate**: Measured every minute. <br> - **Respiration Rate**: Measured every minute. <br> - **Snoring**: Total snoring duration (seconds) per minute. <br> - **SDNN 1**: Standard deviation of heart rate over a one-minute window. <br> - **Timestamp**: Timestamp of each record. |
| **N/A**       | **Demographics**      | - **Sex**: Male or Female. <br> - **Age Group**: One of three age groups: [70–79], [80–89], [90–99]. <br> - **PHQ-9, GDS-15, GAD-7 Scores**: Total score and individual question scores. <br> - **Assessment Date**: Date each assessment was taken. <br> - **Essential Hypertension**: True or False. <br> - **Osteoarthritis**: True or False. |



## Running the code
We have provided raw data and guidelines on how to access, aggregate, and visualise the dataset. The Jupyter Notebooks have been developed using Python 3.9. 
For reproducing the code, an Anaconda virtual environment is also included. The virtual environment can be created using the following line of code in the Anaconda Terminal:
```
conda env create -f resilien.yml
```
After creating and activating the virtual environment, each notebook can be run individually. Please unzip the `Sleepmat_Watch_Data.zip` in the data folder before running the notebooks.

*  *  *  *  *


