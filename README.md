# MRI-Diffusion
Exploring diffusion modelling as a method for interpolation and extrapolation on human brain MRI image data.

## Hyper Parameters
# num_decoders
This parameter defines how many corruption blocks and Unets will exist in the model.

# decoder_depth
This parameter defines how many layers of downsampling/upsampling the Unet has.

# decoder_channels
This parameter defines how many channels the decoder has when it initially does convolution on the image.

# img_dim
This parameter defines the size of the image. The images are assumed to be square images.

# img_channels
This parameter defines how many channels the image has.

# batch_size
This parameter defines the batch size in the training loop.

# corruption_channels
This parameter takes in an array. Each element of the array is meant to represent a channel that will be corrupted. So [0, 2, 4] would corrupt channels 1, 3 and 5.