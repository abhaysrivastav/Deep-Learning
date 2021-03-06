# Autoencoder

* Unsupervised Learning
* Representation Learning
* Impose a bottleneck in the network
* Bottleneck forces a compressed represntation of the input.
## Assumption
* High degree of correlation/structure exist in the data.
* For uncorrelated data(input data that are independent), then the compression and subsequent reconstrction would be difficult.

## Variant of Autoencoders:
1. **Undercomplete Autoencoder**
2. **Sparse Autoencoder**
3. **Denoising Autoencoder**
4. **Contractive Autoencoder**
5. **Convolutional Autoencoder**

### How it is different from PCA?


### Layer by Layer Autoencoding

![](/Autoencoder/docs/Autoencoderlayerbylayer1.PNG "Layer By Layer Auto-encoding")

![](/Autoencoder/docs/Autoencoderlayerbylayer2.PNG "")


### End to End Auto-encoding


### Sparse Autoencoder
* Interesting features can be learnt even when number of nodes in hidden layer is large. 
* Introduce sparsity contraint on the hidden layer that penalize activations within a layer.
* Network learns encoding-decoding that relies on activating a smalll number of neurons.

 *Regularizing Activations not the weight* 
 
 ### Denoising Autoencoder 
 * The Autoencoder learns a generalizable encoding-decoding scheme.
 * **An Approch** :- While training use corrupt data as input but output is uncorrupted original data.
 * The model can not memorize data as input and target output is not same any more.
 * Model learns a vector field to map the input data towards a low dimentional manifold.
