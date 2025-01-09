---
title: "Comparative analysis of cross flow and jet impingement techniques of
heat sink in electronics cooling"
collection: publications
category: manuscripts
permalink: /publication/2010-10-01-paper-title-number-2
excerpt: 'Cooler electronics, smarter solutions: A head-to-head study of cross flow vs. jet impingement for efficient heat sink design.'
date: 2022-08-23
venue: 'Materials Today: Proceedings'
paperurl: '/files/Comparative Analysis of Cross Flow and Jet Impingement of Heat Sink in Electronics Cooling-compressed.pdf'
citation: 'Deerajkumar Parthipan, Et al. :  Comparative analysis of cross flow and jet impingement techniques of heat sink in electronics cooling - 2022'
image: '/publications/jet_vs_cross.png'
---

## Abstract
This study investigates the performance of two advanced cooling techniques—cross flow and jet impingement—for thermal management in heat sinks for electronics. Computational fluid dynamics (CFD) simulations were used to analyze key thermal parameters, including Nusselt number, pressure drop, and pumping power. Results demonstrate that the cross flow technique significantly outperforms jet impingement in terms of thermal efficiency, achieving a 14.5°C lower base temperature on average and requiring 61% less pumping power. The findings are crucial for optimizing thermal management in high-power-density electronics.

## Introduction
The rapid miniaturization of electronics has led to higher power densities, necessitating efficient cooling mechanisms to manage heat dissipation. This study addresses this challenge by comparing the thermal performance of cross flow and jet impingement cooling techniques. The primary focus is on heat sinks, which act as passive heat exchangers to maintain operating temperatures within safe limits, thereby improving the performance and longevity of electronic devices.

## Problem Statement
Despite advancements in electronics cooling, comparative studies on cross flow and jet impingement techniques are limited. This research aims to provide a comprehensive analysis of their thermal characteristics, focusing on parameters such as:
- Nusselt number.
- Base temperature.
- Pressure drop.
- Pumping power requirements.

A circular pin fin heat sink with specific geometrical parameters is used as the test model for this investigation.

## Methodology
### Geometry and Meshing
- **Cross flow:** Rectangular channel geometry with fins placed downstream of the inlet.
- **Jet impingement:** A box-shaped domain with a jet directed at the center of the pin fin array.
- Mesh sensitivity analysis ensured optimal grid size for computational accuracy.

### CFD Simulations
- Simulations were conducted using ANSYS Fluent with the realizable k-ε turbulence model.
- Boundary conditions were set for steady-state, incompressible flow.

### Validation
- The methodology was validated against previous experimental and numerical studies with deviations under 2%.

## Results and Discussion
### Thermal Efficiency
- Cross flow demonstrated superior Nusselt numbers, 41.1% higher than jet impingement, indicating better heat transfer performance.
- Jet impingement showed localized cooling at the heat sink center, while cross flow provided uniform cooling.

### Base Temperature
- Cross flow achieved significantly lower base temperatures across all Reynolds numbers, with an average reduction of 14.5°C compared to jet impingement.

### Pumping Power and Pressure Drop
- Jet impingement required 61% more pumping power due to higher inlet pressure requirements.
- Cross flow had consistently lower pressure drops, reducing energy consumption.

### Grid Independence
- Grid sensitivity analysis revealed minimal variations in results for medium and fine meshes, ensuring computational reliability.

## Conclusion
- Cross flow is more efficient than jet impingement across all tested Reynolds numbers, providing higher thermal performance, lower base temperatures, and reduced energy requirements.
- Jet impingement, while less efficient overall, shows potential for improvement at higher Reynolds numbers.

## Significance
This research provides a foundational comparison of two key cooling techniques, offering valuable insights for the design and optimization of heat sinks in high-power electronics. The results highlight the potential for cross flow cooling to address thermal management challenges in modern devices.

## Authorship
- **Deerajkumar Parthipan:** CFD simulations, methodology, validation, and manuscript preparation.
- **Deepakkumar Rajagopal:** Conceptualization, supervision, and editorial review.

## Acknowledgments
This work was supported by the Computational Fluid Dynamics Laboratory, Department of Thermal and Energy Engineering, VIT Vellore.
