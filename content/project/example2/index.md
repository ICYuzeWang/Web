---
title: Robotic guidance and localization during endoluminal procedures​
summary: Deep Learning, Camera Localisation, Medical Robotics, Medical Imaging
tags:
  - Deep Learning
date: '2016-04-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

links:
  - icon: Slides
    name: Slides
    url: uploads/DL.pdf
  - icon: Codes
    name: Codes
    url: https://github.com/ICYuzeWang/DL_Camera_Localisation.git
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: uploads/VR.pdf
---

In the realm of medical endoscopy, particularly bronchoscopy, the precision of camera pose estimation is paramount. This research delves into this critical aspect, leveraging the power of deep learning to enhance the accuracy and reliability of such estimations. At the heart of this endeavor is a modified PoseNet architecture, integrated with ResNet34 for feature extraction, aiming to accurately predict a 6D Degree of Freedom (DoF) vector. This vector is crucial as it encapsulates both the position and orientation of the camera, a necessity for navigating the complex and narrow pathways of the lung.

The research is grounded in a methodical approach, utilizing synthetic images generated from various centrelines within a 3D lung model. These images are instrumental in training the deep learning model, providing a diverse and comprehensive dataset that challenges and refines the model's capabilities. The training process itself is a testament to the meticulous nature of the study, incorporating not just a variety of centrelines to ensure generalizability but also experimenting with sequential models. These sequential models are pivotal in maintaining temporal consistency in the predictions, a factor that cannot be overstated in the dynamic environment of bronchoscopy.

One of the standout features of this research is the introduction and application of the Heaviside Loss function. This novel approach specifically targets the reduction of out-of-lung prediction errors, a common and critical challenge in previous methodologies. The effectiveness of this function is not merely theoretical but is quantified in the significant reduction of such errors, thereby enhancing the practical applicability of the model in real-world scenarios.

The results of this study are both impressive and quantifiable. The enhanced accuracy in pose estimation is evident in the substantial decrease in the range of errors, as demonstrated by error histograms and per-frame error analysis. This reduction is not just in terms of numbers but also in the increased reliability of the pose estimation, a factor that directly translates to improved navigation during medical procedures. The success of the sequential models further cements this achievement, ensuring that the predictions are not only accurate but consistently so over time.

Moreover, the comprehensive analysis of uncertainties – both aleatoric and epistemic – adds another layer of depth to the study. By calculating and combining these uncertainties, the research provides a more nuanced understanding of the model's prediction reliability, an aspect often overlooked in similar studies.

In conclusion, this research represents a significant advancement in the field of medical endoscopy. By harnessing the capabilities of deep learning and innovatively applying them to the challenge of camera pose estimation in bronchoscopy, the study not only achieves remarkable results in terms of accuracy and reliability but also paves the way for future advancements. It sets a precedent for further research, particularly in refining loss functions and exploring advanced optimization techniques, potentially revolutionizing the application of these techniques in clinical settings.
