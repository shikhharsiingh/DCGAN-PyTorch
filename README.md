# DCGAN-PyTorch
DCGANs are short for Deep Convolutional Generative Adversarial Networks. These work on the same adversarial nature of the generator and discrimnator only that instead of simple model, Convolutions and Convolution Transpose layers are used.
Here, we have implemented DCGAN in PyTorch on the MNIST Dataset.

## Dataset
The dataset can be downloaded from the following [link](http://yann.lecun.com/exdb/mnist/)
<br>
However, PyTorch does provide the facility to download the MNIST dataset in its dataset module. As done in the code, model_DCGAN.py
<br>
<img src = "https://github.com/shikhharsiingh/DCGAN-PyTorch/blob/master/images/sample.png" alt = "/images/sample.png" height = 400></img>

## Model
The model consists of a Generator and a Discriminator. 
The Generator generates images from a vector of random number from a normal distribution. The Discriminator is a CNN classifier.
### Model Architecture
<img src = "https://github.com/shikhharsiingh/DCGAN-PyTorch/blob/master/images/Model_desc.png" alt = "/images/model_desc.png" height = 350></img>
<p>Note: The architecture is not generic and is hardcoded for the MNIST dataset's images.</p>

## Training
Since the GAN is adversarial, the number of epochs will improve the model and the losses of both the Discriminator and Generator will seem to oscillate.
### Training...
<img src = "https://github.com/shikhharsiingh/DCGAN-PyTorch/blob/master/images/train_visuals.png" alt = "/images/train_visuals.png" height = 500></img>

## Results
### After training for 20 epochs
<img src = "https://github.com/shikhharsiingh/DCGAN-PyTorch/blob/master/images/20epochs.png" alt = "/images/20epochs.png" height = 300></img>
<br/>
<img src = "https://github.com/shikhharsiingh/DCGAN-PyTorch/blob/master/images/20ep_res.png" alt = "/images/20ep_res.png" height = 400></img>
### After training for 50 epochs
<img src = "https://github.com/shikhharsiingh/DCGAN-PyTorch/blob/master/images/50epochs.png" alt = "/images/50epochs.png" height = 300></img>
<br>
<img src = "https://github.com/shikhharsiingh/DCGAN-PyTorch/blob/master/images/50ep_res.png" alt = "/images/50ep_res.png" height = 400></img>
### After training for 100 epochs
<img src = "https://github.com/shikhharsiingh/DCGAN-PyTorch/blob/master/images/100epochs.png" alt = "/images/100epochs.png" height = 300></img>
<br>
<img src = "https://github.com/shikhharsiingh/DCGAN-PyTorch/blob/master/images/100ep_res.png" alt = "/images/100ep_res.png" height = 400></img>