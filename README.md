# Unsupervised Anomaly Detection Via Cross Distillation Based on State Space Model

# Introduction
As shown in the figure below, we show several examples of anomaly detection in industrial images, from top to bottom: original image, label overlaid on original image, heat map of detection result.  

![Introduction](/Image/IAD_Introduction.jpg)

# Overview Framework of CDA
The proposed CDA is a knowledge distillation model for anomaly detection in industrial images. Its main components are as follows: a pre-trained teacher encoder (https://arxiv.org/abs/1605.07146) and a MAMBA-based (https://arxiv.org/abs/2312.00752) student decoder.
The main process of CDA is shown in the figure below.  

![Overview framework of CDA](/Image/Overview_framwork.jpg)
# Differences between cross distillation and traditional modes
The following figure shows the differences and advantages between the proposed cross distillation paradigm and the traditional knowledge distillation method.
Compared with traditional distillation methods, CDA introduces a simple cross-distillation paradigm, making full use of the information flow between teachers and students at different stages to promote knowledge transfer.  

![Differences](/Image/distiallation_way.jpg)

# Results
## Quantitative analysis
|| Model || I-AUROC || P-AUROC || PRO  ||
|| PFM   || 97.5    || 97.4    || 93.0 ||
|| CDA   || 98.1    || 97.8    || 93.3 ||

  
## Visualization
The test results of CDA for some categories on the MVTec AD dataset are shown here.


# Conclusion



