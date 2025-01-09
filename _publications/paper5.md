---
title: "Reimplementation of Learning to Reweight Examples for Robust Deep Learning"
collection: publications
category: academics
permalink: /publication/2015-10-01-paper-title-number-3
excerpt: 'Revolutionizing AI training: Tackling noisy and imbalanced data with robust reweighting for smarter deep learning.'
date: 2024-08-01
paperurl: '/files/ECE_50024_Final_Report1.pdf'
image: '/publications/reweight_conf.png'
---

## Abstract
This research reimplements and evaluates the "Learning to Reweight Examples" methodology proposed by Ren et al. (2018), which addresses the challenges of noisy labels and class imbalances in training deep neural networks (DNNs). By integrating meta-learning with online weight approximation, this work demonstrates the effectiveness of reweighting techniques for improving model robustness. Experiments on toy problems and real-world datasets, including CIFAR-10 and HAM10000, confirm the approach’s ability to handle noisy and imbalanced datasets, achieving superior results compared to traditional stochastic gradient descent (SGD) methods.

## Introduction
Deep neural networks are widely used for complex tasks such as image recognition and medical diagnosis. However, their performance is often compromised by noisy labels and imbalanced datasets, leading to overfitting. Current solutions, like hyperparameter tuning and reweighting based on loss values, face challenges in scenarios involving both noisy and imbalanced data. This study addresses these challenges by reimplementing the meta-learning-based reweighting algorithm to dynamically adjust example weights during training.

## Problem Statement
Training datasets with noisy labels and class imbalances result in suboptimal model performance:
- **Noisy Labels:** Arise from insufficient information, subjective classification, or human error.
- **Class Imbalance:** Leads to models disproportionately favoring overrepresented classes, neglecting minority classes.

Existing methods to address these issues often conflict. For example, techniques for noisy data favor examples with lower loss, while methods for imbalanced data prioritize higher-loss examples. This work reexamines these challenges using meta-learning and a representative validation set to guide the reweighting process.

## Methodology
### Meta-Learning Objective
- Optimize example weights to minimize validation loss.
- Use online gradient descent to approximate weights dynamically during training.

### Implementation
- A toy problem with the CIFAR-10 dataset to validate the approach.
- A real-world problem using the HAM10000 dataset for skin lesion classification.

### Algorithm Workflow
- Compute training and validation loss using automatic differentiation.
- Optimize weights to balance class representation and reduce noisy data effects.

### Experimental Setup
- Models trained with reweighting, traditional SGD, and a weighted random sampler for comparison.
- Fine-tuned ResNet50 as the base model for real-world tasks.

## Results
### Toy Problem (CIFAR-10)
- The reweighted model outperformed traditional SGD, achieving higher accuracy as class imbalance increased.
- Demonstrated robust performance across biased training datasets.

### Real-World Problem (HAM10000)
- The reweighted model achieved a balanced multi-class accuracy of 65.56%, outperforming weighted sampling (16.69%) and unweighted training (14.07%).
- Improved class-wise accuracy, particularly for underrepresented classes, as shown in confusion matrices and detailed metrics.

### Comparative Analysis
- The dynamic reweighting algorithm effectively handled class imbalances and noisy labels, surpassing baseline methods.
- Training times increased due to additional forward and backward passes but were justified by improved performance.

## Significance
This work extends the original methodology by applying it to a real-world medical dataset, showcasing its utility in practical scenarios like automated diagnosis systems. The reweighted approach provides a promising framework for addressing noisy and imbalanced datasets, paving the way for more robust machine learning applications in critical fields such as healthcare.

## Conclusion
The reweighting algorithm successfully enhances model robustness against noisy and imbalanced datasets, outperforming traditional and baseline methods. While the implemented model did not match top-performing results in the ISIC Challenge, further experimentation and resource optimization could bridge the gap. This study underscores the potential of meta-learning approaches in improving training efficiency and accuracy for challenging datasets.

## Authorship
- **Deerajkumar Parthipan:** Implementation, experimentation, and manuscript preparation.
- **Parth Patil:** Algorithm development and analysis.
- **Ben Boardley:** Code optimization and dataset preparation.
- **Jack Gardner:** Validation and experimental setup.
- **Emily Loiselle:** Documentation and editorial review.
