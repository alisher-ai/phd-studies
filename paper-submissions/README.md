In this folder I am collecting all the documents related to paper submissions.

# Human Action Recognition

- Datasets: UCF-101 | HMDB-51 | Kinetics | AVA | ActivityNet | STAIR | HACS | NTU


## Related works - 3D CNN
1. [PAPER: Temporal 3D ConvNets: New Architecture and Transfer Learning for Video Classification](https://arxiv.org/pdf/1711.08200.pdf)
      - temporal transition layer
      - extend (2D) DenseNet with 3D filters and pooling kernels
      - transfer the knowledge from 2D CNN to initialize 3D CNN

<p align="center"> <img src="https://github.com/alisher-ai/phd-studies/blob/main/figures/temporal-3d-convnets.png" width="500" /> </p>
  
2.  [PAPER: Learning Spatio-Temporal Features with 3D Residual Networks for Action Recognition](https://arxiv.org/pdf/1708.07632.pdf)
      - 3D ResNets pre-trained on Kinetics dataset
      - Train deeper networks such as ResNet to get better performance and not to overfit 
3.  [PAPER: Can Spatiotemporal 3D CNNs Retrace the History of 2D CNNs and ImageNet?](https://arxiv.org/pdf/1711.09577.pdf)
      - Examines the various 3D CNN archutecture, from shallow to very deep, performances on current video datasets. 
      - ResNet-18: significant overfitting for UCF-101, HMDB-51, and ActivityNet but not for Kinetics.
      - The Kinetics dataset has sufficient data for training of deep 3D CNNs, and enables training of up to 152 ResNets layers
      - ResNeXt-101 achieved 78.4% average accuracy on the Kinetics test set. 
      - Kinetics pretrained simple 3D architectures outperforms complex 2D architectures, and the pretrained ResNeXt-101 achieved 94.5% and 70.2% on UCF-101 and HMDB-51, respectively.

4.  [CODE: Convolutional Autoencoder](https://github.com/udacity/deep-learning-v2-pytorch/tree/master/autoencoder/convolutional-autoencoder)
5.  [BLOG POST: Deep Learning for Videos: A 2018 Guide to Action Recognition](https://blog.qure.ai/notes/deep-learning-for-videos-action-recognition-review)
6.  [PAPER: Large-scale Video Classification with Convolutional Neural Networks](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42455.pdf)
7.  [CODE: 3D-ResNets-PyTorch](https://github.com/kenshohara/3D-ResNets-PyTorch)
8.  [PAPER: Human Action Recognition using Factorized Spatio-Temporal Convolutional Networks](https://arxiv.org/pdf/1510.00562.pdf)
      - Factorization of spatio-temporal convolutional networks is proposed
      - Factorize the original 3D convolution kernel learning as a sequential process of learning 2D spatial kernels in the lower layers (called spatial convolutional layers), followed by learning 1D temporal kernels in the upper layers (called temporal convolutional layers).
      - Introduced a novel transformation and permutation (T-P) operator to form an intermediate layer of the proposed network --> handling 1D convolution (which supposed to deal with temporal dimension) with 2D convolutions in T-F (time and filters) dimensions.
      - To address the issue of sequence alignment, we pro- pose a training and inference strategy based on sam- pling multiple video clips from a given action video sequence.



## Related works - DTW
1. [D3TW: Discriminative Differentiable Dynamic Time Warping for Weakly Supervised Action Alignment and Segmentation](https://openaccess.thecvf.com/content_CVPR_2019/papers/Chang_D3TW_Discriminative_Differentiable_Dynamic_Time_Warping_for_Weakly_Supervised_Action_CVPR_2019_paper.pdf)
2. [The Globally Optimal Reparameterization Algorithm: an Alternative to Fast Dynamic Time Warping for Action Recognition in Video Sequences](https://arxiv.org/abs/1807.05485)
3. 


## Contributions
1. train 3D CNN with 2D CNN feature maps rather than using raw spatial data. This method would store the temporal information as it is and decrease the spatial dimensions of the data.
2. DTW + 3D CNN --> classification 
