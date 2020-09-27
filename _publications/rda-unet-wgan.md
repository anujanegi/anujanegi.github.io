---
layout: publication
title: RDA-UNET-WGAN - An Accurate Breast Ultrasound Lesion Segmentation Using Wasserstein Generative Adversarial Networks
authors: <b>Anuja Negi</b>, Alex Noel Joseph Raj, Ruban Nersisson, Zhemin Zhuang, M Murugappan
publication: Arabian Journal for Science and Engineering
year: 2020
doi: https://doi.org/10.1007/s13369-020-04480-z
---

> Segmentation results of the RDA-UNET-WGAN. Column (a), (b) and (c) denote
the breast ultrasound image, the ground truth mask and predicted segmentation mask with various regions marked respectively. Regions
marked in purple represent the intersection of predicted segmentation and the ground truth, red represents the lesion area not
predicted as lesion and blue represents the non-lesion regions classified as lesion by the model.

# Abstract

Early-stage detection of lesions is the best possible way to fight breast cancer, a disease with the highest malignancy ratio among women. Though several methods primarily based on deep learning have been proposed for tumor segmentation, it is still a challenging problem due to false positives and the precise boundary detection required for segmentation. In this paper, we propose a Generative Adversarial Network (GAN) based algorithm for segmenting the tumor in Breast Ultrasound images. The GAN model comprises of two modules: generator and discriminator. Residual-Dilated-Attention-Gate-UNet (RDAU-NET) is used as the generator which serves as a segmentation module and a CNN classifier is employed as the discriminator. To stabilize training, Wasserstein GAN (WGAN) algorithm has been used. The proposed hybrid deep learning model is called the WGAN-RDA-UNET. The model is assessed with several quantitative metrics and is also compared with existing methods both quantitatively and qualitatively. The overall Accuracy, PR-AUC, ROC-AUC and F1-score achieved were 0.98, 0.95, 0.89 and 0.88 respectively which are better than most conventional deep net models. The results also showcase the shortcomings of CNN, RDA U-Net and other models and how they can be rectified using the WGAN-RDA-UNET model.
