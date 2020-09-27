---
layout: publication
title: Eye State Detection for use in Advanced Driver Assistance Systems
authors: Shubham Sharma, <b>Anuja Negi</b>, Shantanu Singh, Dinesh Samuel Sathia Raj, Jasmine S. Graceline, V. Vaidehi, Subramaniam Ganesan
publication: International Conference on Recent Trends in Advance Computing
year: 2018
doi: https://doi.org/10.1109/ICRTAC.2018.8679348
---
# Abstract

Most automobiles lack reliable smart systems that can constantly track the driver's behaviour and raise alarms as required. Extant systems are either too slow or not robust enough to cope with different types of drivers and conditions. In this paper, a robust system to continuously track the driver's eye and detect its state (open/close) is proposed. Frames from a live camera feed are constantly processed. Viola Jones algorithm, using Haar filters extracts the eye. The extraction is efficient with and without spectacles (translucent) and the system can even estimate the Region of Interest (RoI) where it is most likely to find the eye in the event that no eyes are explicitly detected. A trained CNN model using the LeNet architecture classifies the extracted eyes. The rate at which predictions are made is also higher than existing systems. The system raises an alarm if, after analysing the data points, it detects any anomalies.