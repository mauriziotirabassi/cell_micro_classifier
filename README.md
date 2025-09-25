# White Blood Cell Microscopy Classifier

The project focuses on multi-class classification of WBC images, replacing manual feature engineering with automatic feature extraction from pretrained convolutional networks. The pipeline includes data cleaning, imbalance handling, augmentation, and model interpretability.

## Dataset

- 13,759 images, 96×96×3, 8 classes  
- Outliers removed using t-SNE feature analysis  
- Balanced test set to ensure unbiased evaluation

## Approach

- Transfer learning with multiple CNN architectures (e.g., EfficientNetV2M, ResNet50, VGG16)  
- Weighted loss and data augmentation to address class imbalance  
- Grad-CAM used for model interpretability  
- Performance compared across models and augmentation strategies

## Results

- Best local F1 score: 98.75%  
- Best online score: 85%  
- Final model: EfficientNetV2M + custom dense classifier
