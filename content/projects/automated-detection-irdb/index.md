---
title: "Automated detection of isolated REM sleep behavior disorder using computer vision"
date: 2025-10-10
summary: "A computer-vision pipeline using conventional 2D sleep-lab cameras to automatically detect iRBD from REM movement dynamics with up to 91.9% accuracy."
authors:
  - "Mohamed Abdelfattah"
  - "Li Zhou"
  - "Oliver Sum-Ping"
  - "Anahid Hekmat"
  - "Joanna Galati"
  - "Niraj Gupta"
  - "George Adaimi"
  - "Salonee Marwaha"
  - "Ankit Parekh"
  - "Emmanuel Mignot"
  - "Alexandre Alahi"
  - "Emmanuel During"
venue: "Annals of Neurology 2025"
card_authors:
  - "Mohamed Abdelfattah"
  - '<a href="https://scholar.google.com/citations?user=Mm_I4s4AAAAJ&hl=zh-CN" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>Li Zhou</authorname></a>'
  - '<a href="https://stanfordhealthcare.org/doctors/s/oliver-sumping.html" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>Oliver Sum-Ping</authorname></a>'
  - '<a href="https://med.stanford.edu/profiles/anahid-hekmat" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>Anahid Hekmat</authorname></a>'
  - '<a href="https://www.linkedin.com/in/joanna-galati-9aba03229/" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>Joanna Galati</authorname></a>'
  - '<a href="https://www.linkedin.com/in/niraj-gupta-0425b7133/" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>Niraj Gupta</authorname></a>'
  - '<a href="https://www.georgeadaimi.com" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>George Adaimi</authorname></a>'
  - '<a href="https://www.linkedin.com/in/salonee-marwaha/" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>Salonee Marwaha</authorname></a>'
  - '<a href="https://profiles.icahn.mssm.edu/ankit-parekh" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>Ankit Parekh</authorname></a>'
  - '<a href="https://med.stanford.edu/profiles/emmanuel-mignot" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>Emmanuel Mignot</authorname></a>'
  - '<a href="https://people.epfl.ch/alexandre.alahi?lang=en" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>Alexandre Alahi</authorname></a>'
  - '<a href="https://profiles.mountsinai.org/emmanuel-h-during" target="_blank" rel="noopener" class="text-primary-600 dark:text-primary-400"><authorname>Emmanuel During</authorname></a>'
conference: "Annals of Neurology 2025"
tags:
  - Action Recognition
  - Datasets
tech_stack:
  - Optical Flow
  - Video Polysomnography (vPSG)
  - Movement Feature Engineering
  - Clinical Computer Vision
links:
  - type: paper
    url: https://onlinelibrary.wiley.com/doi/10.1002/ana.27256
    label: Paper
featured: false
status: "Published"
role: "First Author"
duration: "Research Project"
team_size: 12
highlights:
  - "Published in Annals of Neurology (2025)"
  - "2D camera-based automated iRBD detection in clinical sleep labs"
  - "Highest reported accuracy of 91.9% using short-movement analysis"
---

An automated computer-vision approach for detecting isolated REM sleep behavior disorder (iRBD) from overnight video-polysomnography recordings using standard 2D cameras.

## Abstract

### Objective

Isolated rapid eye movement (REM) sleep behavior disorder (iRBD) is, in most cases, an early stage of Parkinson's disease or related disorders. Diagnosis requires an overnight video-polysomnogram (vPSG), however, even for sleep experts, interpreting vPSG data is challenging. Using a 3D camera, automated analysis of movements has yielded high accuracy. We aimed to replicate and extend prior work using a conventional 2D camera.

### Methods

The dataset included 172 vPSG recordings from a clinical sleep center, 81 patients with iRBD and 91 non-RBD healthy controls (63 with a range of other sleep disorders and 28 healthy sleepers). An optical flow computer vision algorithm automatically detected movements during rapid eye movement (REM) sleep, from which features of rate, ratio, magnitude and velocity of movements, and ratio of immobility were extracted.

### Results

Patients with iRBD exhibited an increased number of shorter movements and immobility periods. Accuracies for detecting iRBD ranged from 84.9% (with 2 features) to 87.2% (with 5 features). Combining all 5 features but only analyzing short (0.1-2 second duration) movements achieved the highest accuracy at 91.9%. Of the 11 patients with iRBD without noticeable movements during vPSG, 7 were correctly identified.

### Interpretation

This work improves prior art by using a 2D camera routinely used in sleep laboratories and improving performance by adding only 3 features. This approach could be implemented in clinical sleep laboratories to facilitate and improve the diagnosis of iRBD. Coupled with automated detection of REM sleep, it should also be tested in the home environment using conventional infrared cameras to detect and/or monitor RBD.

## Citation

ANN NEUROL 2025;97:860-872
