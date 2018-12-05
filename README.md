# vae_latent_space
Study latent space dimensionality on reconstruction accuracy in variational autoencoders using Keras and Tensorflow

Repo contains two tests, on MNIST and CIFAR10. Not surprisingly, the more complex data in CIFAR10 requires a higher dimensionality in the latent space reprenentation

VAE_loss is a weighted sum of two losses, the cross-entropy loss and the Kullback-Leibler (KL) divergence which measures how much two distributions diverge from each other. The MNIST plot below shows the effect of changing the weight on the KL divergence. As expected, by increasing the weight, the training loss goes up since the penalty on not adhering to the distribution is higher. However, the accuracy of the reconstructed images remains about the same. 

**MNIST**

![Alt text](mnist_error.png?raw=true "MNIST error")

Latent space of 2 dims:
![Alt text](mnist/2_dim_space.png?raw=true "MNIST 2 dims")

Latent space of 32 dims:
![Alt text](mnist/32_dim_space.png?raw=true "MNIST 2 dims")




**CIFAR10**

![Alt text](cifar10_error.png?raw=true "CIFAR10 error")

Latent space of 32 dims:
![Alt text](cifar10/32_dim_space.png?raw=true "32 dims")

Latent space of 256 dims:
![Alt text](cifar10/256_dim_space.png?raw=true "256 dims")


