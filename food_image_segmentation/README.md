# Food Identification with Segmentation

This project implements food image segmentation using the FoodSeg103 dataset, which contains over 7,000 food images labeled with 103 food categories.

## Approach
- Model DeepLabV3 with ResNet-101 backbone, fine-tuned on FoodSeg103
- Preprocessing resizing, normalization, augmentation (flip, brightness, hue, saturation)

## Results
- Mean IoU 41.69% across classes
- Effective segmentation for clear scenes; performance drops for visually similar or mixed ingredients

## Skills & Tools
Python, PyTorch, DeepLabV3, Semantic Segmentation, Data Augmentation
