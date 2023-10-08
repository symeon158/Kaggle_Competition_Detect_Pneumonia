# Detection of Pneumonia in Chest X-ray Images using Neural Networks

## Authors
- **Savvas Nikolaidis** - [Email](mailto:snikolaidis@ihu.edu.gr)
- **Symeon Papadopoulos** - [Email](mailto:spapadopoulos@ihu.edu.gr)

## Abstract
This repository encompasses a study on the detection of pneumonia in chest X-ray images, utilizing machine learning and specifically, three different approaches: a custom 15-layer CNN model, the VGG19 pretrained model, and an ensemble model.

### Keywords
CNN, Pneumonia, Pretrained Model, Classification, Ensemble

## Table of Contents
1. [Data & Problem Description](#data-problem-description)
2. [Model Descriptions](#model-descriptions)
   - [15-layer CNN](#15-layer-cnn)
   - [VGG19 Pretrained Model](#vgg19-pretrained-model)
   - [Ensemble Model](#ensemble-model)
3. [Comparative Experiments and Results](#comparative-experiments-and-results)
4. [Conclusions](#conclusions)
5. [Getting Started](#getting-started)
6. [Acknowledgements](#acknowledgements)
7. [References](#references)

## 1. Data & Problem Description <a name="data-problem-description"></a>
A dataset of 4672 training and 1168 test chest X-ray images, labeled as 0 (normal), 1 (bacterial pneumonia), or 2 (viral pneumonia), is leveraged to categorize X-ray images into one of three classifications: viral, bacterial, or no pneumonia.

## 2. Model Descriptions <a name="model-descriptions"></a>
### 2.1. 15-layer CNN <a name="15-layer-cnn"></a>
The custom 15-layer CNN model includes 5 Conv2D layers, 5 MaxPooling2D layers, 1 Flatten layer, 4 Dense layers, and 2 Dropout layers.

### 2.2. VGG19 Pretrained Model <a name="vgg19-pretrained-model"></a>
The VGG19 pretrained model was employed and fine-tuned for the specific classification task.

### 2.3. Ensemble Model <a name="ensemble-model"></a>
The ensemble model combines the custom CNN, VGG19, and Xception models but did not outperform the individual models.

## 3. Comparative Experiments and Results <a name="comparative-experiments-and-results"></a>
The models were evaluated based on their stability and performance accuracy during the training and validation phases, with VGG19 exhibiting the highest performance accuracy and notable stability.

## 4. Conclusions <a name="conclusions"></a>
VGG19 emerges as a particularly suitable choice for this image classification task, demonstrating exceptional performance and stability.

## 5. Getting Started <a name="getting-started"></a>
### Prerequisites
- Python
- Tensorflow
- Keras
- Scikit-learn
- Numpy
- CV2
- Pandas

### Usage
1. **Step 1:** Data Preprocessing
   - Image resizing
   - Normalization
   - Augmentation
   
2. **Step 2:** Model Training
   - Train the 15-layer CNN model
   - Train the VGG19 model
   - Train the ensemble model

3. **Step 3:** Model Evaluation
   - Calculate evaluation metrics
   - Compare model performances

### Note
For detailed methodology, model architectures, and experimental setups, refer to the provided Jupyter Notebooks or scripts.

## 6. Acknowledgements <a name="acknowledgements"></a>
- Dataset: Detect Pneumonia (Spring 2023) from Kaggle

## 7. References <a name="references"></a>
Torres A, Serra-Batlles J, Ferrer A, Jiménez P, Celis R, Cobo E, Rodriguez-Roisin R. Severe community-acquired pneumonia. Epidemiology and prognostic factors. Am Rev Respir Dis. 1991;144(2):312–8. doi: 10.1164/ajrccm/144.2.312. [PubMed] [CrossRef] [Google Scholar]
