---
layout: default
---

# 2019 Master Thesis: Anomaly Detection in Time Series Data with Neural Networks  

[@Fraunhofer EMFT Munich](https://www.emft.fraunhofer.de/)  
![emft_logo](./images/emft_logo.jpg)  

Tags: Machine Learning, Deep Learning, Anomaly Detection, Time Series Data  

- [1. Abstract](#1-abstract)
- [2. Content](#2-content)
- [3. Reference](#3-reference)

___

## 1. Abstract  

For the implementation of preventive maintenance in production environments, this
thesis extends an anomaly detection approach whose performance is evaluated using
time series data from processes of different complexity.  

Sensor data of a wide range of process parameters are becoming increasingly available.
For the processing of large amounts of data, the application of machine learning methods
is state of the art. The absence of information about all potential error patterns of the
process data limits the choice of compatible methods.  

The anomaly detection method learns the normal process cycles from the time series data
of successfully completed processes. Autoencoders, adapted structures of neural
networks, learn to reconstruct these training data. The optimized reconstruction
capability of normal processes is essential for the detection of deviating processes.
Statistical methods, based on the reconstruction error distribution of normal and
anomalous validation data, are used to further optimize the anomaly detection
performance.  

This extended approach is applied against different datasets. The procedure comprises
data preprocessing, model design, model training and the evaluation and optimization of
the anomaly detection performance.  

The applied datasets confirm the practical applicability of the extended anomaly
detection procedure. However, more complex process data reveal the limitations of
simple autoencoder models.  

___

## 2. Content

**Preventive Maintenance (PvM):**  
Maintenance activities are only to be performed when actually needed. Unexpected breaks and unexploited equipment lifetime are minimized
simultaneously  
![emft_predictive_maintenance](./images/emft_predictive_maintenance.png)  

**Anomaly Detection:**  
Anomaly Detection is the problem of finding patterns in data that do not follow the expected behavior. Anomalies are unusual data instances that should be further analyzed to identify the cause of its occurrence.  
![emft_anomaly_detection](./images/emft_anomaly_detection.png)  

**Time Series Data:**  
Time Series Data in production environments is data from sensors sampled in a sequential order and usually recorded at regular intervals.  
![emft_time_series_data](./images/emft_time_series_data.png)  

**Autoencoder:**  
Autoencoders are feedforward networks with sequential layers of neuronal units. The input data is to be reconstructed at the output layer. The information exchange is constrained by the specific network architecture.  By using only unlabeled data, autoencoders learn the encoding of information independently. Hence, they are considered an unsupervised learning approach.  
![emft_autoencoder](./images/emft_autoencoder.png)  

**Time Series Data Anomaly Detection:**  
an anomaly classifier is defined using statistical methods based on the reconstruction performance of the trained autoencoder model  
![emft_threshold](./images/emft_threshold.png)  
![emft_threshold_confusion](./images/emft_threshold_confusion.png)  

**Reconstruction Error:**
The trained autoencoder model is evaluated according to its reconstruction performance based on normal and anomalous input data  
![emft_reconstruction_error](./images/emft_reconstruction_error.png)  
![emft_reconstruction_error_density](./images/emft_reconstruction_error_density.png)  

**Optimum F-Beta Threshold:**
The optimum F-Beta threshold is determined using validation data applied to classify normal and anomalous test data  
![emft_optimum_threshold](./images/emft_optimum_threshold.png)  
![emft_optimum_threshold_confusion](./images/emft_optimum_threshold_confusion.png)  
![emft_performance_parameters](./images/emft_performance_parameters.png)  

___

## 3. Reference

![emft_zeugnis](./images/emft_zeugnis.png)  

___

[back](./)
