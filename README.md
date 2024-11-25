# Advanced Image Classification Framework

This repository implements a comprehensive framework for image classification, leveraging state-of-the-art deep learning models and attention mechanisms. The pipeline includes data preprocessing, model training, evaluation, and explainability using LIME.

## Features

### Data Loading and Augmentation
- Dynamic loading of train, validation, and test datasets.
- Augmentation techniques like rescaling, flipping, and shifting for robust training.

### Pretrained Models
- Includes models such as:
  - **CoAtNet**
  - **ResMLP**
  - **WaveMLP**
  - **MobileViT**
  - **SwinTransformer**
  - **Beit**
- Pretrained weights (`ImageNet`) for transfer learning.

### Custom Architectures
- **Attention Mechanisms**: Integration of custom linear attention layers.
- **Ensemble Modeling**: Combining predictions from multiple models.
- **VGG19 with Attention**: Enhanced with a self-attention layer.

### Training and Callbacks
- Optimized training using callbacks:
  - `ModelCheckpoint`: Saves the best-performing model.
  - `ReduceLROnPlateau`: Adjusts learning rate dynamically.
  - `EarlyStopping`: Stops training when validation performance plateaus.

### Evaluation
- Metrics: Accuracy, AUC, Precision, Recall, Cohen’s Kappa, F1-Score.
- Visualizations:
  - Confusion Matrix.
  - ROC Curves with AUC for each class.

### Explainability with LIME
- **LIME**: Highlights regions influencing model predictions.
- **Boundary Visualization**: Marks areas in images contributing to decisions.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/image-classification-framework.git
