## Resilient Dataset

- [Resilient Dataset](#description)
  * [Data description](#description)
  * [Running the code](#running-the-code)
  
# Description
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.16755408.svg)]([https://doi.org/10.5281/zenodo.16755408]) 
<br/>

The RESILIENT Dataset: Multimodal Monitoring of Ageing-Related Multi-Morbidities and Cognitive Decline.
The dataset is available on its corresponding [Zenodo repository](https://doi.org/10.5281/zenodo.15045662).
<!--The full description of this dataset is published in Nature Scientific Data: [paper](https://doi.org/10.1038/s41597-023-02519-y)-->

The dataset is provided for research purposes and supporting patient care. 

Please acknowledge the Surrey and Borders Partnership NHS Foundation Trust and Howz in any publication or use of this dataset. 

The RESILIENT dataset is organised into four main components: 1) a CSV file containing demographic information and baseline assessments related to mental health and cognitive functioning for all participants; 2) a metadata CSV files describing variables present in the demographic and devices data; 3) a CSV summary file providing per-participant data coverage statistics, including the number of recorded days, average records per day, and the earliest and latest timestamps; and 4) individual participant folders containing raw time-series data, including sleep states and physiological features captured by sleep mats, as well as step counts and heart rate data recorded by smart watches. More specifically, there are four tables included in each participant folder: ScanWatch Steps, ScanWatch HeartRate, Sleep States, and Sleep Physiology. Each folder is named after the participant's unique identifier (UID), allowing cross-referencing between the device data and the demographic information.
### Summary of Data Tables and Recorded Variables

| **Device**     | **Table Name**         | **Variables** |
|--------------|----------------------|------------------------------------------------------------------|
| **ScanWatch** | **Steps**            | - **Steps**: Number of steps recorded per hour. <br> - **Timestamp**: Timestamp of each record. |
|              | **Heart Rate**        | - **Heart Rate**: Measurements taken every 10 minutes. <br> - **Timestamp**: Timestamp of each record. |
| **Sleep Mat** | **Sleep States**      | - **Sleep State**: One of four sleep states (Light, Deep, REM, Wake up). <br> - **Start Timestamp**: Start time of the corresponding sleep state. <br> - **End Timestamp**: End time of the corresponding sleep state. |
|              | **Sleep Physiology**   | - **Heart Rate**: Measured every minute. <br> - **Respiration Rate**: Measured every minute. <br> - **Snoring**: Total snoring duration (seconds) per minute. <br> - **SDNN 1**: Standard deviation of heart rate over a one-minute window. <br> - **Timestamp**: Timestamp of each record. |
| **N/A**       | **Demographics**      | - **Sex**: Male or Female. <br> - **ACE-III Scores**: Total scores at baseline and 6-month follow-up with individual item scores. <br> - **PHQ-9, GDS-15, GAD-7 Scores**: Total score at baseline and individual question scores. <br> - **Assessment Date**: Date each assessment was taken. <br> - **Essential Hypertension**: True or False. <br> - **Osteoarthritis**: True or False. |



## Running the code
We have provided raw data and guidelines on how to access, aggregate, and visualise the dataset. The Jupyter Notebooks have been developed using Python 3.9. 
For reproducing the code, the required Python packages can be installed using the following line of code:
```
pip install -r requirements.txt
```
Please download the data from [Zenodo repository](https://zenodo.org/records/15877645) and unzip the `Sleepmat_Watch_Data.zip` in the data folder before running the code.

*  *  *  *  *


