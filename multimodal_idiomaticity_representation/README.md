# Multimodal Idiomaticity Representation

This project explores multimodal idiom understanding, aiming to match idioms in a sentence to the image that best represents their intended meaning. By combining visual and linguistic cues, the goal is to enhance computational comprehension of figurative language.

## Approach
- Data Augmentation: Used T5-small to generate diverse captions for improved generalization.  
- Zero-shot CLIP: Matched text-based idioms with images without explicit training.  
- Fine-tuned CLIP: Enhanced performance using original and augmented datasets.  
- Evaluation Metrics: Accuracy, F1 Score, Precision, Recall.

## Results
- Zero-shot CLIP: 33.33% accuracy, 100% recall, low F1 score due to bias toward idiomatic predictions.  
- Fine-tuned CLIP (original dataset): 81.48% accuracy, F1 score 61.54%, best performance overall.  
- Fine-tuning with augmented data: Mixed results; unfreezing multiple layers led to overfitting, reducing accuracy.

Key Insights:  
- LLM-augmented data can improve robustness.  
- Fine-tuning outperforms zero-shot predictions for task-specific performance.  
- Multimodal learning (text + image) enhances understanding of visually intuitive idioms.

## Skills & Tools
Python, PyTorch, CLIP, T5-small, NLP, Multimodal Learning, Data Augmentation, Model Evaluation
