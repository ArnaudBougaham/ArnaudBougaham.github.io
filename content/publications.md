---
title: "Publications & Projects"
date: 2025-01-27
draft: false
translationKey: "publications"
---

## Publications

### 2025

**"GENQUAD : Generative Models and Quality Constraints for Anomaly Detection: Application to Industrial and Medical Images"**
- **Author**: Arnaud Bougaham
- **Type**: Ph.D. Thesis
- **Institution**: University of Namur
- **Supervisors**: Prof. Benoît Frénay, Prof. Isabelle Linden
- **Date**: December 2025
- **Description**: Doctoral thesis proposing a deep-learning framework for anomaly detection in safety-critical domains, focusing on minimal supervision and human-aligned interpretability. This work is a development of generative models to meet quality constraints for anomaly detection in industrial and medical imaging applications.
- **Link**: [Institutional Repository](https://pure.unamur.be/ws/portalfiles/portal/114586556/2025_BougahamA_these.pdf)

**"Towards Photonic Band Diagram Generation with Transformer-Latent Diffusion Models"**
- **Authors**: V. Delchevalerie, N. Roy, A. Bougaham, A. Mayer, B. Frénay, M. Lobet
- **Type**: arXiv preprint
- **Date**: October 2025
- **Description**: Research on using transformer-latent diffusion models for generating photonic band diagrams, combining deep learning with photonics applications.
- **Link**: [arXiv:2510.01749](https://arxiv.org/abs/2510.01749)

**"Towards a Trustworthy Anomaly Detection for Critical Applications through Approximated Partial AUC Loss"**
- **Authors**: Arnaud Bougaham, Benoît Frénay
- **Type**: arXiv preprint
- **Date**: February 2025
- **Description**: Presents a method applying an approximated partial AUC ROC loss through a neural network classifier, targeting critical applications requiring minimal false positives while ensuring zero false negatives. The approach optimizes a specific critical range of the AUC ROC curve.
- **Link**: [arXiv:2502.11570](https://arxiv.org/abs/2502.11570)


### 2024

**"Industrial and Medical Anomaly Detection Through Cycle-Consistent Adversarial Networks"**
- **Authors**: A. Bougaham, V. Delchevalerie, M. E. Adoui, B. Frénay
- **Journal**: Neurocomputing, Volume 614, Article 128762
- **Date**: October 2024
- **Description**: Explores the application of cycle-consistent adversarial networks in detecting anomalies in both industrial and medical images, enabling cross-domain anomaly detection.
- **Link**: [Elsevier](https://www.sciencedirect.com/science/article/pii/S0925231224015339?casa_token=Woj5X3ESxtkAAAAA:fbXVIZgaqOh_83CHOmTxYpRwh9st6mom2OCvTTshYH87pv_VoHP_AqdCQn5V0TvHZTmFUFGmXg)

### 2023

**"Composite Score for Anomaly Detection in Imbalanced Real-World Industrial Dataset"**
- **Authors**: Arnaud Bougaham, Mohammed El Adoui, Isabelle Linden, Benoît Frénay
- **Journal**: Machine Learning, Volume 113, Issue 7, Pages 4381-4406
- **Date**: November 2023
- **Description**: Presents a composite scoring method for anomaly detection in imbalanced industrial datasets, addressing challenges in real-world manufacturing applications.
- **Link**: [Springer Nature](https://link.springer.com/article/10.1007/s10994-023-06415-9)

### 2021

**"GanoDIP-GAN Anomaly Detection through Intermediate Patches: a PCBA Manufacturing Case"**
- **Authors**: Arnaud Bougaham, Adrien Bibal, Isabelle Linden, Benoît Frénay
- **Journal**: Proceedings of Machine Learning Research 154:104–117, 2021
- **Date**: September 2021
- **Description**: A method for anomaly detection using intermediate patches, applied to Printed Circuit Board Assembly (PCBA) manufacturing. Addresses challenges in imbalanced learning domains.
- **Link**: [Proceedings of Machine Learning Research](https://proceedings.mlr.press/v154/bougaham21a/bougaham21a.pdf)


## Conference Presentations & Posters

### 2025

**"Quality Constrained Anomaly Detection through an Approximated Partial AUC Loss"**
- **Event**: Mardi des Chercheurs 2025
- **Location**: Valenciennes, France
- **Date**: April 1, 2025
- **Description**: Presentation on quality-constrained anomaly detection methods using partial AUC approximations for high-stakes applications. Addresses anomaly detection in critical applications, focusing on minimizing false positives while ensuring zero false negatives.
- **Link**: [Research Portal](https://pure.unamur.be/ws/portalfiles/portal/108839834/Poster_ARB_Mardi_Chercheurs_2025_A0.pdf)

### 2024

**"Generative Models and Quality Constraints for Anomaly Detection: Application to Industrial and Medical Images"**
- **Event**: Mardi des Chercheurs 2024
- **Location**: Mons, Belgium
- **Date**: March 26, 2024
- **Description**: Poster presentation on generative models and quality constraints for anomaly detection in industrial and medical imaging applications.
- **Link**: [Research Portal](https://pure.unamur.be/ws/portalfiles/portal/92983052/Poster_ARB_Mardi_Chercheurs_A0.pdf)

### 2023

**"Quality and Performance Optimization through Generative Adversarial Networks based Anomaly Detection"**
- **Author**: Arnaud Bougaham
- **Event**: 21st Symposium on Intelligent Data Analysis (IDA 2023)
- **Date**: April 14, 2023
- **Description**: Presentation on using Generative Adversarial Networks for anomaly detection to optimize quality and performance in industrial applications.
- **Link**: [Research Portal](https://pure.unamur.be/ws/portalfiles/portal/81393314/Poster_ARB_IDA_A0_final.pdf)

### 2021

**"GanoDIP-GAN Anomaly Detection through Intermediate Patches: a PCBA Manufacturing Case"**
- **Authors**: Arnaud Bougaham, A. Bibal, Isabelle Linden, Benoît Frénay
- **Event**: Third International Workshop on Learning with Imbalanced Domains: Theory and Applications
- **Date**: September 2021
- **Description**: Presents GanoDIP, a method for anomaly detection using intermediate patches, applied to Printed Circuit Board Assembly (PCBA) manufacturing. Addresses challenges in imbalanced learning domains.
- **Link**: [Proceedings of Machine Learning Research](https://proceedings.mlr.press/v154/bougaham21a/bougaham21a.pdf)


## Open Source Projects

### [tapAUC](https://github.com/ArnaudBougaham/tapAUC)
**Language**: Jupyter Notebook  
**Description**: Towards a Trustworthy Anomaly Detection for Critical Applications through Approximated Partial AUC Loss. A method that dynamically applies a trustworthy approximated partial AUC ROC loss to train binary classifiers that optimize the specific range of the AUC ROC curve, preventing the True Positive Rate (TPR) from reaching 100% while minimizing the False Positive Rate (FPR). Results show a TPR of 92.52% at a 20.43% FPR for an average across 6 datasets.  
**Authos**: Arnaud Bougaham  
**Topics**: Anomaly Detection, Industry 4.0, Industrial Images, Medical Images, High Sensitivity, Partial AUC, Quality Constraints

---

### [CGAN-AD](https://github.com/ArnaudBougaham/CGAN-AD)
**Language**: Python  
**Description**: Cycle-Consistent Adversarial Networks (CycleGANs) for industrial and medical anomaly detection. The system learns to transform between normal and abnormal image domains, enabling effective anomaly detection through reconstruction error analysis. Supports multiple datasets including brain MRI, breast cancer, OCT, pathology, and industrial defect detection (screws, wood, tiles, hazelnuts). Published research paper at Neurocomputing.  
**Research Paper**: ["Industrial and Medical Anomaly Detection Through Cycle-Consistent Adversarial Networks"](https://www.sciencedirect.com/science/article/pii/S0925231224015339) - Neurocomputing  
**Author**: Arnaud Bougaham  
**Topics**: GANs, CycleGAN, Anomaly Detection, Computer Vision, Deep Learning, Medical Imaging, Industrial Imaging, Domain Translation

---

### [Pinkcc25_Ovsegft_ARB](https://github.com/ArnaudBougaham/Pinkcc25_Ovsegft_ARB)
**Language**: Python  
**Description**: 1st Prize PinkCC Challenge 2025 - Ovarian Cancer Segmentation using nnUnet pretrained (OVSEG Fine-Tuned). Complete pipeline for ovarian cancer segmentation achieving a combined score of 0.7026 (Dilated Dice Score and F2). Features include fine-tuning with domain adaptation, progressive patch size training strategy (16×96×96 to 24×160×160), dynamic batch size management, and optimized learning rates. Built upon the OVSEG framework with technical modifications for challenge-specific optimization.  
**Achievement**: First Place in PinkCC Challenge 2025  
**Author**: Arnaud Bougaham  
**Topics**: Medical Imaging, Computer Vision, Transformers, Segmentation, Deep Learning, Ovarian Cancer, Foundation Models, Domain Adaptation

---

### [Clustering](https://github.com/ArnaudBougaham/Clustering)
**Language**: Jupyter Notebook  
**Description**: TimeSeries → Tabular → 2D → Cluster → Distance → Anomaly Detection. A comprehensive pipeline for clustering algorithms and distance metrics applied to time series and tabular data, with applications in anomaly detection.  
**Author**: Arnaud Bougaham  
**Topics**: Clustering, Machine Learning, Data Analysis, Time Series, Anomaly Detection, Distance Metrics

---

### [TP_ML](https://github.com/ArnaudBougaham/TP_ML)
**Language**: Jupyter Notebook  
**Description**: Machine Learning practical work for steel industry applications. Teaching materials and exercises covering energy consumption analysis, prediction models, clustering for consumption profiles, and visual anomaly detection using deep learning (VAE). Includes four comprehensive labs with Google Colab integration for hands-on learning.  
**Author**: Arnaud Bougaham  
**Topics**: Education, Machine Learning, Teaching Materials, Industrial Applications, Energy Analysis, Anomaly Detection, Deep Learning

---

### [Photonics2Pix](https://github.com/ArnaudBougaham/Photonics2Pix)
**Language**: Python  
**Description**: Research and development project focusing on photonics applications (Band Diagram generation from physical material).  
**Author**: Arnaud Bougaham  
**Topics**: Photonics, Research, Applied Physics

## Media Contributions

### Video

**"Ph.D. Defense: GENQUAD - Generative Models and Quality Constraints for Anomaly Detection"**
- **Date**: December 11, 2025
- **Event**: Ph.D. Defense at University of Namur
- **Description**: Full recording of the Ph.D. thesis defense presenting "Generative Models and Quality Constraints for Anomaly Detection: Application to Industrial and Medical Images". The defense covers the complete research work on developing deep-learning frameworks for anomaly detection in safety-critical domains, including generative models, quality constraints, and applications in industrial and medical imaging.
- **Link**: [Google Drive](https://drive.google.com/file/d/1U821PSJEy71ySDH1i7sZjlMjd-FlIil6/view)

**"Draw My PhD: L'IA au service de l'humain dans le milieu industriel, mythe ou réalité?"**
- **Date**: May 2, 2024
- **Description**: Video presentation discussing the role of AI in enhancing quality control within the automotive industry, focusing on the development of generative models and computer vision tools for effective quality control.
- **Link**: [YouTube](https://www.youtube.com/watch?v=adqfS7gL9Vc) EN subtitled

**"Meetup GenAI - Développement de modèles génératifs destinés à satisfaire des contraintes qualités"**
- **Date**: June 4, 2025
- **Event**: Meetup GenAI (Flint)
- **Description**: Presentation on generative models for quality-constrained anomaly detection in critical applications (industrial and medical domains). The method uses GANs with discretized vectors to transform images into their "anomaly-free" versions, followed by neural network classification optimized on a critical range of the AUC ROC curve. This research is designed for implementation in industrial quality control and disease detection (radiology, nuclear medicine), with a strong focus on practical applications related to data and business constraints.
- **Link**: [YouTube](https://www.youtube.com/watch?v=Y8wo3InfmrE)

### Podcasts

**"Thèse ? Antithèse ? Synthèse !"**
- **Description**: Guest appearance discussing the experience of returning to academia for a PhD after years in the professional world, sharing insights on balancing industry experience with academic research.
- **Link**: [Spotify](https://creators.spotify.com/pod/profile/these-antithese-synthese/episodes/18---GENERAL---Faire-une-thse-longtemps-aprs-ses-tudes--mission-impossible-e2hpllh)
