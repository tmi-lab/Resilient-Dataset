## Resilient Dataset

- [Resilient Dataset](#description)
  * [Data description](#description)
  * [Running the code](#running-the-code)
  
# Description
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15045663.svg)]([https://doi.org/10.5281/zenodo.15045663]) 
<br/>

The RESILIENT Dataset: Multimodal Monitoring of Ageing-Related Multi-Morbidities and Cognitive Decline.
The dataset is available on its corresponding [Zenodo repository](https://zenodo.org/record/15045663).
<!--The full description of this dataset is published in Nature Scientific Data: [paper](https://doi.org/10.1038/s41597-023-02519-y)-->

The dataset is provided for research purposes and supporting patient care. 

Please acknowledge the Surrey and Borders Partnership NHS Foundation Trust and Howz in any publication or use of this dataset. 

The RESILIENT dataset is organised into two components: 1). one CSV file containing demographic information and baseline assessments related to mental health and cognitive ability for all participants; 2). individual folders that contain raw data, including sleep state and physiological features recorded by sleep mats, as well as step counts and heart rate from smart watches. More specifically, there are four tables included in each participant folder: ScanWatch Steps, ScanWatch HeartRate, Sleep States, Sleep Physiology. Due to differences in sampling frequencies, these variables are recorded in separate tables. Each folder is named after the participant's unique identifier (UID), allowing cross-referencing between the device data and the demographic information. 
### Summary of Data Tables and Recorded Variables

| **Device**     | **Table Name**         | **Variables** |
|--------------|----------------------|------------------------------------------------------------------|
| **ScanWatch** | **Steps**            | - **Steps**: Number of steps recorded per hour. <br> - **Timestamp**: Timestamp of each record. |
|              | **Heart Rate**        | - **Heart Rate**: Measurements taken every 10 minutes. <br> - **Timestamp**: Timestamp of each record. |
| **Sleep Mat** | **Sleep States**      | - **Sleep State**: One of four sleep states (Light, Deep, REM, Wake up). <br> - **Start Timestamp**: Start time of the corresponding sleep state. <br> - **End Timestamp**: End time of the corresponding sleep state. |
|              | **Sleep Physiology**   | - **Heart Rate**: Measured every minute. <br> - **Respiration Rate**: Measured every minute. <br> - **Snoring**: Total snoring duration (seconds) per minute. <br> - **SDNN 1**: Standard deviation of heart rate over a one-minute window. <br> - **Timestamp**: Timestamp of each record. |
| **N/A**       | **Demographics**      | - **Sex**: Male or Female. <br> - **PHQ-9, GDS-15, GAD-7 Scores**: Total score and individual question scores. <br> - **Assessment Date**: Date each assessment was taken. <br> - **Essential Hypertension**: True or False. <br> - **Osteoarthritis**: True or False. |



## Running the code
We have provided raw data and guidelines on how to access, aggregate, and visualise the dataset. The Jupyter Notebooks have been developed using Python 3.9. 
For reproducing the code, the required Python packages can be installed using the following line of code:
```
pip install -r requirements.txt
```
Please download the data from [Zenodo repository](https://zenodo.org/record/15045663) and unzip the `Sleepmat_Watch_Data.zip` in the data folder before running the code.

*  *  *  *  *


