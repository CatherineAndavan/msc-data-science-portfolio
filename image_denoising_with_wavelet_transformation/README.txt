# Image Denoising with Wavelet Transformation

This project implements image denoising using Haar Wavelet Transform. The goal is to remove noise from images by decomposing them into frequency components, thresholding high-frequency noise, and reconstructing the image to improve visual quality.

## Approach
- Data Loading:  
  - Reads PGM (Netpbm grayscale) images and converts them to NumPy arrays for processing  
  - Handles header information (magic number, width, height, max pixel value) and pixel data  

- Wavelet Decomposition:  
  - Performs Forward Discrete Wavelet Transform (FDWT) using Haar wavelets  
  - Separates images into low-frequency (LL) and high-frequency (LH, HL, HH) components  
  - Applies thresholding on high-frequency components to remove noise  

- Image Reconstruction:  
  - Inverse Discrete Wavelet Transform (IDWT) reconstructs images from thresholded components  
  - Evaluates reconstruction quality using Mean Squared Error (MSE)  

- Denoising:  
  - Hard thresholding: keeps coefficients above threshold, sets others to zero  
  - Soft thresholding: shrinks smaller coefficients toward zero  
  - Reconstructed images closely resemble original images while removing noise  

## Results
- Successfully denoised images while preserving important details  
- Demonstrates effectiveness of Haar wavelet transform and thresholding for image preprocessing  
- Provides a foundational approach useful in deep learning tasks such as face recognition or historical image restoration  

## Skills & Tools
Python, NumPy, Matplotlib, Wavelet Transforms, Image Processing, Haar Wavelet, Discrete Wavelet Transform, Thresholding
