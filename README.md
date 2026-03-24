# Neuro-AI: Mapping Artificial Neural Networks to the Human Visual Cortex

## Project Overview
This computational neuroscience project investigates the representational alignment between Artificial Neural Networks (ANNs) and the biological human brain. Using functional magnetic resonance imaging (fMRI) data, this pipeline evaluates how well different layers of a deep learning vision model predict neural activity in highly specialized regions of the human visual cortex.

## Target Brain Regions (ROIs)
The encoding models are evaluated across three distinct Regions of Interest:
* **FFA (Fusiform Face Area):** Processes facial recognition.
* **PPA (Parahippocampal Place Area):** Processes environmental scenes and landscapes.
* **EBA (Extrastriate Body Area):** Processes the visual perception of human bodies.

## Methodology: Ridge Regression Encoding Models
Instead of using AI to *diagnose* a disease, this project uses AI as a *computational model of the brain*. 
1. **Feature Extraction:** Visual stimuli are passed through a pre-trained ANN. Activation features are extracted from 5 distinct mid-to-late layers to capture complex spatial representations.
2. **Brain-Score Mapping:** A Ridge Regression model is trained to map the high-dimensional ANN features to the biological voxel responses in the human brain.
3. **Evaluation:** The models are tested on a strictly held-out human subject. Performance is measured via Pearson correlation to determine which specific layer of the artificial network best mathematically mirrors the functional processing of the biological tissue.

## Tech Stack
* `Python`, `Google Colab`
* `Scikit-Learn` (Ridge Regression modeling and cross-validation)
* `NumPy`, `Pandas` (High-dimensional matrix operations)
* `Matplotlib`, `Seaborn` (Data visualization and Brain-Score plotting)

---
*Created by Tanvi Gambhir as an exploration into Neuro-AI, Brain-Computer Interfacing, and visual encoding models.*
