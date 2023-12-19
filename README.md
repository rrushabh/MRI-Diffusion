# MRI-Diffusion
Exploring diffusion modelling as a method for interpolation and extrapolation on human brain MRI image data.

This notebook lays out the diffusion model architecture used, as well as a training loop to train the model with implemented learning rate and corruption noise scheduling. The corruption_channels parameter allows the user to specify the type of training experiment they wish to carry out. Indexes can be specified to corrupt specific slices in the input set of 5 consecutive MRI images. This is a flexible approach to carrying out training for multiple different objectives, such as interpolation, extrapolation and pure image generation.

# Hyper Parameters
## num_decoders
This parameter defines how many corruption blocks and Unets will exist in the model.

## decoder_depth
This parameter defines how many layers of downsampling/upsampling the Unet has.

## decoder_channels
This parameter defines how many channels the decoder has when it initially does convolution on the image.

## img_dim
This parameter defines the size of the image. The images are assumed to be square images.

## img_channels
This parameter defines how many channels the image has.

## batch_size
This parameter defines the batch size in the training loop.

## corruption_channels
This parameter takes in an array. Each element of the array is meant to represent a channel that will be corrupted. So [0, 2, 4] would corrupt channels 1, 3 and 5.
