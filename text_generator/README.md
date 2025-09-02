# Text Generator

This project implements a text generation model inspired by Agatha Christie's writing style. The goal is to generate coherent text based on a seed prompt using recurrent neural networks.

## Approach
- Data Preprocessing:  
  - Removed special characters (except period and apostrophe)  
  - Converted text to lowercase  
  - Tokenized into sentences using `sent_tokenize`  
  - Padded sequences for uniform input length  

- Model Architecture:  
  - Embedding layer to convert words into vectors  
  - 3-layer LSTM (Long Short-Term Memory) network to capture long-term dependencies  
  - Normalization layer to prevent overfitting  
  - Early stopping with patience = 3 to halt training if validation loss increases  

- Techniques to Improve Output:  
  - Adjusting temperature to increase diversity  
  - Adding more LSTM or Bidirectional LSTM layers  
  - Increasing training data with more texts  
  - Transfer learning from pre-trained text generator models  

## Example Output
Seed text: `"There was a murder in the building"`  

Generated text:  
> There was a murder in the building point about your not too that s was temporary sold heeds of poirot i packet our look was drawer i or the which fianc influence concerning street the my table house match number from of hastings out very arm do to that seen the sad but fibre  

Comparison with ChatGPT:  
> There was a murder in the building. The body lay motionless in the dimly lit hallway, a crimson pool spreading across the floor. The residents whispered in hushed tones, eyes darting with suspicion. Inspector Graves arrived, his gaze sharp. "Locked doors. No forced entry. The killer is among us."

## Skills & Tools
Python, TensorFlow/Keras, LSTM, RNN, NLP, Text Preprocessing, Sequence Modeling
