# Face Translation using CycleGAN

This project implements a Cycle-Consistent Generative Adversarial Network (CycleGAN) to translate human faces into animal faces and vice versa, without requiring paired training data. The goal is to generate realistic images in the target domain while preserving core features of the original images.

## Approach
- Data Preparation:  
  - Human faces from CelebA and UTK Face Cropped datasets  
  - Animal faces from a cat_dog dataset  
  - Organized into `humans` and `animals` folders  

- Data Preprocessing:  
  - Images resized to 256×256 pixels  
  - Random horizontal flips for data augmentation  
  - Pixel normalization to [-1, 1]  

- Model Architecture:  
  - Two generators: human→animal, animal→human  
  - Two discriminators: human images, animal images  
  - Optimizes adversarial loss for realism and cycle-consistency loss for reversible translation  

- Training:  
  - Trained on unpaired datasets  
  - Outputs visualized to show translation quality  

## Results
- The model successfully translates faces between human and animal domains.  
- Translated images retain core features while convincingly adopting target domain characteristics.  
- Demonstrates unpaired image translation and CycleGAN’s effe
