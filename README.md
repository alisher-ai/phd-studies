# Alisher Abdulkhaev's PhD Studies
- The University of Tsukuba
- Supervisor: Kazuhiro Fukui
- Period: 2020.04 -- 2023.04

# General schema
Data Efficient Deep Learning
<p align="center"> <img src="https://github.com/alisher0717/phd-studies/blob/main/figures/schema.png" width="1000" /> </p>

## Abbreviations
- **CL**: Curriculum Learning
- **CoL**: Contrastive Learning
- **ML**: Meta Learning
- **FA**: Image Augmentations in Fourier Domain
- **SSL**: Self-Supervised Learning
- **WA**: Weight Averaging
- **GT**: Gradient Tracking
- **TD**: Task Design

## Experiment ideas:
### [FA](https://github.com/alisher0717/phd-studies/blob/main/FourierDomain.md)
* Phase/Wavelet scrambling
* Mask design
* Hybrid Images

* FA --> train SSL pipeline with proposed augmentations 

### TD
* Task Design: find various unsupervised/self-supervised tasks for representation learning
* TD --> train SSL pipeline with FA augmentations

### CL
* Curriculum Learning with designed tasks (from easy towards hard tasks). 
* CL with TD --> support with FA --> SSL
