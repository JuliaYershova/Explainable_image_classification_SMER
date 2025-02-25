# SMER+LLM for Explainable Image Classification 🚀

This repository contains the code and experiments, which focuses on enhancing explainability in image classification. The project integrates the SMER (Self Model Entities Rated) method with Large Language Models (LLMs) to provide high-fidelity, object-level explanations.

## Overview
### SMER+LLM Workflow: 
Combines SMER's direct evaluation of region importance with the interpretative power of LLMs to generate precise bounding boxes and coherent visual explanations. 🔍
1. Get Description of the Images
Extract textual descriptions from the images using image captioning code.[here](https://github.com/PotipJulia/Explainable_image_classification_SMER/blob/main/Get_image_description.ipynb)

2. Get Embeddings and Aggregate
Generate embeddings from the image descriptions and aggregate them for downstream analysis.[here](https://github.com/PotipJulia/Explainable_image_classification_SMER/blob/main/Get_embeddings_and_aggregate.ipynb)

3. Train Logistic Regression, Get Importance Concepts using SMER and LIME, Calculate AOPC  and compare
Train a logistic regression model to predict class labels, then use SMER and LIME to extract importance concepts. Calculate the AOPC metric to evaluate the interpretability of the predictions. [here](https://github.com/PotipJulia/Explainable_image_classification_SMER/blob/main/Train_LR_plot_AOPC.ipynb).

5. Compare SMER+LLM and LIM (based on Logistic Regression).[here](https://github.com/PotipJulia/Explainable_image_classification_SMER/blob/main/LIME_for_images(LR).ipynb).

### Method Comparisons: 
Includes implementations and evaluations of alternative explanation methods such as LIME and MoRF (Most Relevant First). These methods are applied both directly on images and using a ResNet classifier for a comprehensive comparison. ⚖️
- Code for experiments with LIME is [here](https://github.com/PotipJulia/Explainable_image_classification_SMER/blob/main/LIME_for_images(ResNet).ipynb)
- Code for experiment with MoRF is [here](https://github.com/PotipJulia/Explainable_image_classification_SMER/blob/main/MoRF_for_images(ResNet).ipynb)
### Quantitative Evaluation: 
Experiments employ the AOPC (Average Output Probability Change) metric to measure the impact of removing influential features, validating the reliability of our approach. 📊
### Qualitative Evaluation:
Visual comparisons demonstrate that our SMER+LLM workflow delivers more coherent and interpretable object-level explanations compared to existing techniques. 🎨
### Reproducibility: 
All code, data processing scripts, and detailed instructions for reproducing the results are included. 
____________________________
For complete setup instructions, experiment details, and how to replicate our evaluations, please refer to the README.md.
Contributions, feedback, and collaborations are highly welcome. Let's make explainable AI even more exciting! 🎉

Enjoy exploring the repository!
