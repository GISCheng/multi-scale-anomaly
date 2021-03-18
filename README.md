# Multi-scale detection and interpretation of human activity anomalies

## Title: Multi-scale detection and interpretation of spatio-temporal anomalies of human activities represented by time-series

## Abstract
Spatio-temporal patterns of human activities can be affected by events, such as extreme weather. They cause anomalies that could be expressed by abnormal activity patterns deviating from the inherent ones. The detection of spatio-temporal anomalies thus helps to understand the implicit influencing mechanism with which the external factors affect human activities. Existing methods of spatio-temporal anomaly detection usually treat the temporal information as attributes of spatial units, which is an over-simplification as it ignores complicated temporal patterns (e.g., periodic components of time-series). Moreover, as the spatio-temporal resolutions affect expressed characteristics of anomalies, the sensitivity of anomalies to scale is also worth investigating. This study intends to detect and interpret the spatio-temporal anomalies of human activities from a multi-scale perspective. Different from the single-scale consideration and independent consideration of multiple scales, this research investigates how the anomalies' characteristics change at multiple scales by anomaly matching. The matching criteria are the overlapping degree of spatio-temporal influence ranges of anomalies. It helps to specify the events that caused the expressed anomalies. Besides, we introduce the time-series decomposition methods to decompose complicated temporal patterns, highlighting the abnormal changes in activity patterns. The study is validated using a multi-temporal-scale simulation experiment, and a multi-spatial-scale experiment based on taxi data in Beijing. Results show that the multi-scale method can detect various anomalies. Moreover, obtained multi-scale characteristics of anomalies are easy to compare with external data thus benefit anomaly interpretation (validated by two sample anomalies). This study highlights the significance of scales in anomaly detection of human activities and provides references for related works.

## Statement
The program of the time-series decomposition is developed based on the previous implementation of STL in GitHub ([STLDecompose](https://github.com/jrmontag/STLDecompose)).

## Code description
1. The file "Multi-temporal-scale.ipynb" is the program of the simulation of multi-temporal-scale anomaly detection (Section 3.1 of the article).

2. The file "Multi-spatial-scale.ipynb" is the demo program of the multi-spatial-scale anomaly detection experiment based on sample data (Section 3.2 of the article, except for the time-series organization).

## Data description
The file "input_threescales" is the input of the program "Multi-spatial-scale.ipynb". It is saved as the byte format and can be read by the pickle library of Python. The file records the sample time-series data of taxi origin point volume at three spatial scales. Each line records the information of one spatial unit. The data fields include ID, son nodes' IDs, TAS (temporal activity signatures), taxi origin point volume, father node's ID, and the quadtree ID.

## Cite
Please consider citing our paper if this helps in your work:
