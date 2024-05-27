# CNC-Machine-Clustering-Anomaly-Detection

✨Takeaway:

Anomaly detection in CNC-machined parts using Gaussian Mixture Models. 
This project clusters parts based on their dimensions and identifies anomalies within each cluster to help engineers diagnose issues with CNC machines. 



✨Project Description
- This project focuses on detecting anomalies in parts produced by three different computerized numerical control (CNC) machines. Each part has two critical dimensions (X1 and X2) measured. The parts are mixed and not identified by the machine that produced them.

✨Objectives:
- Cluster Analysis: First, I will look for any cluster patterns to group parts potentially produced by the same CNC machine.
Anomaly Detection: Then, I will try to identify the anomalies in each machine (the 5% of the parts whose dimensions differ from the majority of the parts produced by the same machine). This will help the engineer analyze each machine separately so they can diagnose the issues with each CNC machine.

✨Methodology:
- Data Loading and Preprocessing: I will load the dataset containing measurements of 1251 parts and store it in a pandas DataFrame. Then, I'll extract the relevant dimensions (X1 and X2) into a NumPy array.
Visualization: I will create scatter plots to visualize the distribution of the parts' dimensions.
- GMM Clustering: I'll fit a Gaussian Mixture Model (GMM) to the data to identify clusters, each likely representing parts from the same CNC machine. I'll compute and plot the centroids of the clusters.
- Cluster Assignment: I will assign data points to clusters and visualize each cluster with a different color.
Anomaly Detection: Using the GMM, I'll identify anomalies within each cluster based on a density threshold, marking the lowest 5% of data points as anomalies. These anomalies will be visualized on the scatter plot.


<img width="536" alt="Screen Shot 2024-05-27 at 1 56 44 PM" src="https://github.com/ZTECH10/CNC-Machine-Clustering-Anomaly-Detection/assets/53150477/60b41d50-84bc-4acc-bd26-bfaee858a8cb">
