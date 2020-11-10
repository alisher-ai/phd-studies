## 2020.11.04 - 2020.11.11

### Partial Fourier frequency images
### Dataset: fashion MNIST

### Experiments
1. feed the images in different domains: 
 - f^0 (pixel images) --> CNN1 
 - f^0.5 (partial fourier domain) --> CNN2
 - f^1 (fourier domain) --> CNN3
 
2. concatenate input tensors to regular CNN (number of channels: 5)
 - RGBMP (RGB + Phase + Magnitude) --> CNN
 
3. concatenate input tensors to regular depthwise separable CNN (number of channels: 5)
 - RGBMP (RGB + Phase + Magnitude) --> (depthwise separable) CNN
 
4. late fusion scenario:
 - RGB --> CNN1 --> feat1
 - MP --> CNN2 --> feat2
 - [feat1, feat2] --> predictions
