---
title: "Analysis of a Modified SIR Model for COVID-19 Transmission Dynamics"
collection: publications
category: academics
permalink: /publication/2015-10-01-paper-title-number-3
excerpt: 'Unveiling pandemic dynamics: A time-delayed SIR model to decode COVID-19 transmission and guide smarter interventions.'
date: 2024-08-01
slidesurl: 'http://academicpages.github.io/files/slides3.pdf'
paperurl: 'http://academicpages.github.io/files/paper3.pdf'
image: '/publications/case2_10.9934_circle.png'
---

## Abstract
This study proposes and analyzes a modified Susceptible-Infected-Recovered (SIR) model to capture the dynamics of COVID-19 transmission, incorporating a time delay in the transmission rate. The model examines the stability of disease-free and endemic equilibria and the impact of time delays on system behavior, including potential oscillations. Numerical simulations validate the theoretical findings, offering insights into the long-term dynamics of COVID-19 transmission and the effects of interventions such as social distancing and vaccination.

## Introduction
The COVID-19 pandemic has significantly impacted global health and economies, necessitating accurate models to understand and mitigate disease spread. The classical SIR model, while widely used, overlooks critical factors such as delays in transmission dynamics. This paper extends the SIR framework by introducing a time delay and reducing the model to two compartments—susceptible (S) and infected (I)—to simplify calculations and focus on key transmission dynamics.

## Problem Statement
Traditional SIR models fail to address:
- Delays between infection and detection.
- Dynamic behaviors such as oscillations due to intervention delays.

This study modifies the SIR model to incorporate these factors, aiming to analyze their effects on transmission stability and long-term dynamics.

## Methodology
### Model Formulation
- Modified SIR model with time delay in the transmission rate.
- Reduced to susceptible and infected compartments for simplicity.

### Key Parameters
- Transmission rate (β), recovery rate (γ), carrying capacity (k), and delay (τ).

### Stability Analysis
- Disease-free equilibrium (DFE) and endemic equilibrium (EE) were derived.
- Linear stability analysis was conducted to assess equilibrium stability under varying reproduction numbers (ℜ₀).

### Numerical Simulations
- Simulated using MATLAB's `dde23` solver for delay differential equations.
- Investigated dynamics under different delay scenarios.

## Results
### Equilibrium Analysis
- DFE is stable when ℜ₀ < 1, implying successful containment.
- EE becomes unstable for delays exceeding a critical value (τ₀), leading to oscillatory behavior.

### Time Delay Impact
- For τ < τ₀, the system stabilizes around the EE.
- For τ > τ₀, Hopf bifurcations occur, generating periodic oscillations.

### Case Studies
- **Case 1:** ℜ₀ < 1 demonstrated asymptotic stability at DFE.
- **Case 2:** ℜ₀ > 1 showed the onset of oscillations for delays beyond τ₀.

### Numerical Insights
- Critical time delays and their role in destabilizing equilibria were identified.
- Simulation trajectories validated theoretical findings.

## Conclusion
The modified SIR model highlights the critical role of time delays in COVID-19 transmission dynamics. Key findings include:
- Stability conditions for DFE and EE.
- The emergence of oscillations due to delays.
- Practical implications for designing timely interventions, such as quarantine and vaccination schedules.

## Significance
This study provides a robust framework for analyzing infectious disease dynamics, emphasizing the effects of delays and their implications for public health strategies. Future extensions could include additional compartments, such as vaccinated or exposed populations, and optimization based on real-world data.

## Authorship
- **Deerajkumar Parthipan:** Model development, stability analysis, simulations, and manuscript preparation.
