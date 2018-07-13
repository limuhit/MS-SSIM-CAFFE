# MS-SSIM-CAFFE
CUDA  MS-SSIM loss for caffe framework.

This code only implement the gpu version of the MS-SSIM with the CUDNN. The default parameter was used in the code. The image should be transpose to (channel, height, width) as the input. The value of the image should be in the range of [0,255]. As a simple version, we do not considering the image with the size less than the $16\times11$. Because the convolutional kernel should be reset for downsampled image with a size less than 11. In the extreme condition, we should guarentee the image after down-sampling 16 times should be large than or equalto $11\times11$.  
