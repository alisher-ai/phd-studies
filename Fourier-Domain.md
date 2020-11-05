# Fourier Domain Classification/Augmentation
## Readings
- fractional Fourier Transform (FRFT): transform a function to any intermediate domain between time/space and frequency
- Heisenberg's Uncertainty Principle: position and the velocity of an object cannot both be measured exactly, at the same time
- [The Uncertainty Principle in Image Processing](https://sci-hub.do/https://ieeexplore.ieee.org/document/4767599)

## Experiments:
### 1. Image classification with Fourier Images and RGB images
#### 1. MP (Magnitude & Phase) images--> CNN --> classifier
#### 2. Concatenate RGB and MP (Magnitude & Phase) channels --> CNN --> classifier
#### 3. Concatenate RGB and MP (Magnitude & Phase) channels --> Depthwise Separable CNN --> classifier
#### 4. Process RGB and MP images in parallel --> concatenate the features (logits) --> classifier
 
