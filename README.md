# CSE 5717: Big Data Analytics Project (GeoGuessr / GeoVision)

**Team Members:** Layla Nassar and Nina Cunha

## Project Overview

GeoVision is a machine learning project inspired by GeoGuessr. Our goal is to investigate whether a model can identify the country where a street-view image was captured using visual information alone. We want to explore how features such as road markings, architecture, signs, vegetation, landscapes, and infrastructure can help distinguish locations around the world.

Rather than predicting an exact address or geographic coordinate, we plan to approach this as a **multiclass image classification** problem: given a street-view image, the model will predict the country in which it was taken.

## Project Goals

- Explore publicly available, country-labeled street-view image datasets, including options on **Hugging Face**.
- Prepare image data for training and evaluation while considering differences in country representation and image quality.
- Investigate machine learning and deep learning techniques for recognizing geographic patterns in images.
- Compare model performance and examine which visual characteristics may help or confuse country predictions.
- Develop a model that can make country-level predictions on street-view images it has not seen before.

## Models and Approach Under Consideration

We plan to explore **transfer learning** with pretrained convolutional neural networks (CNNs). Potential architectures include **ResNet-18** and **MobileNetV2**. We may also use pretrained image embeddings with traditional classifiers as baseline comparisons, and investigate fine-tuning if appropriate.

Our general workflow will involve selecting a suitable dataset, preprocessing images, developing and comparing models, and evaluating predictions using metrics such as **accuracy, precision, recall, F1-score, and confusion matrices**. We also hope to analyze common mistakes, especially when countries have similar landscapes or infrastructure.

## Expected Outcome

By the end of the project, we aim to have a working country-classification pipeline and a comparison of different modeling approaches. Beyond prediction accuracy, we hope to better understand how effectively machine learning can identify geographic clues from street-view imagery and where it struggles.

**Project Status:** GeoVision is currently in development. Dataset selection, the final list of countries, model architectures, and experimental methods may change as we explore and test different options.