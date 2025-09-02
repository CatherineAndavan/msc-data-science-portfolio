# Fine-Grained Bird Species Classification

This project implements a fine-grained image classification model to identify bird species from images, focusing on subtle differences between visually similar classes.

## Approach
- Data Preprocessing:  
  - Images resized to 256×256, batch size 32  
  - Data augmentation: flipping, rotation, zoom, contrast adjustment  
  - One-hot encoding for 20 bird species classes  
  - Efficient loading using `AUTOTUNE` for efficient training  

- Model Architecture & Training:  
  - Transfer Learning with EfficientNetV2-S (pre-trained on ImageNet)  
  - Added GlobalAveragePooling2D, Dropout (0.3), and Dense softmax output layer  
  - Fine-tuned last 50 layers to adapt to dataset  
  - Optimizer: Adam, Loss: Categorical Cross-Entropy  
  - Trained on 40% of images, validated on 10%, tested on 50%  

- Evaluation Metrics:  
  - Accuracy: 90.62%  
  - Precision: 93.52%  
  - Recall: 90.28%  
  - Confusion matrix indicates most classes are well-classified  

## Future Improvements
- Explore alternative architectures: DenseNet121, Vision Transformers (ViT), GANs  
- Model ensembles or stacking  
- Hyperparameter tuning (learning rate, batch size, dropout)  
- Experiment with optimizers like AdamW or SGD  
- Train on larger datasets for better generalization  

## Skills & Tools
Python, TensorFlow/Keras, EfficientNet, Image Preprocessing, Data Augmentation, Fine-Tuning, Transfer Learning, Classification Metrics
