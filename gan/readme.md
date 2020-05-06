## Homework 4:  Implicit Models [1]
In this homework, GAN network is trained on CIFAR-10 dataset using pytorch. Implemented network follows SN-GAN [2] CIFAR Resnet architecture. <br>
### Content
1. WGAN-GP.ipynb includes implementing and training the following variations of WGAN-GP [3] on CIFAR.<br>
  * WGAN-GP, batch size=128.
  * WGAN-GP, with ResBlocks in generator using 128 filters instead of 256 filters but trained
with a larger batch size 256 instead of 128.
  * WGAN-GP, with self-modulated batch-normalization [4] in the generator
2. inception_cifar10.ipynb includes training Inception architecture classifier from scratch on CIFAR-10. Trained network is used to calculate Inception Score for for all networks in wgan notebook.
### Results
The following slideshows contains GAN samples over training epochs.
1. WGAN-GP trained with batch size 128 and 256 filters in generator.<br>
  ![alt text](wgan_128.gif "")
2. WGAN-GP trained with batch size 256 and 128 filters in generator.<br>
  ![alt text](wgan_256.gif "")
3. WGAN-GP with self-modulated batchnorm.<br>
  ![alt text](wgan_mod.gif "")


#### References
1. Homework 4 https://drive.google.com/file/d/1vBJro462ax_Pk4SN9TJdzNUN0vnRV0r-/view
2. Takeru Miyato et al. “Spectral normalization for generative adversarial networks”. In: arXiv
preprint arXiv:1802.05957 (2018).
3. Ishaan Gulrajani et al. “Improved training of wasserstein gans”. In: Advances in Neural
Information Processing Systems. 2017, pp. 5767–5777.
4. Ting Chen et al. “On self modulation for generative adversarial networks”. In: arXiv preprint
arXiv:1810.01365 (2018).

