## IMAGE UPSCALING ALGORITHM

# SRCNN
Implementation of SRCNN in PyTorch.

# Usage

To train the model with a zoom factor of 2, for 200 epochs and on GPU:

`python main.py --zoom_factor 2 --nb_epoch 200 --cuda`

At each epoch, a `.pth` model file will be saved.

To use the model on an image: (the zoom factor must be the same the one used to train the model)

`python run.py --zoom_factor 2 --model model_199.pth --image example.jpg --cuda`

# Example

Original image:

![Original image](1_SRCNN\images\input\1_original.jpg "Original image")

Bicubic interpolation zoom:

![Bicubic interpolation zoom](1_SRCNN\images\2_bicubic.jpg "Bicubic interpolation zoom")

SRCNN zoom:

![ SRCNN zoom](1_SRCNN\images\3_srcnn.jpg "SRCNN zoom")

# FSRCNN

Under Construction

# Reference

[Original paper on SRCNN by Dong et al. (*Image Super-Resolution Using Deep Convolutional Networks*)](http://personal.ie.cuhk.edu.hk/~ccloy/files/eccv_2014_deepresolution.pdf)

[Accelerating the Super-Resolution Convolutional Neural Network by Chao Dong, Chen Change Loy, Xiaoou Tang](http://mmlab.ie.cuhk.edu.hk/projects/FSRCNN.html)
