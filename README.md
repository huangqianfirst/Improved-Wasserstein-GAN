# Improved Wasserstein GAN Tensorflow

Tensorflow implementation of [WGAN-GP](https://arxiv.org/pdf/1704.00028.pdf), Wasserstein GAN with Gradient Penalty.

Datasets
* [CelebA dataset](https://www.dropbox.com/sh/8oqt9vytwxb3s4r/AADIKlz8PR9zr6Y20qbkunrba/Img/img_align_celeba.zip)

___

### How to Run
`python train.py --DATASET=celeba --DATA_DIR=/path/to/celeba/`

Other options include [SELU activations](https://arxiv.org/abs/1706.02515) and
[layer normalization](https://arxiv.org/abs/1607.06450), which the authors of
WGAN-GP suggest, as the discriminator does not use batch normalization because that
would conflict with the gradient penalty.

### Results

![img](http://i.imgur.com/SgXTiDs.jpg)

