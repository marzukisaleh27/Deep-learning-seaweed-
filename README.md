# Deep-learning-seaweed-
## Spectral-Spatial UNet for mapping seaweed cultivation
Spectral-Spatial UNet (SSUNet) model for seaweed cultivation mapping. <br/>
The architecture of SSUNet is composed of several layers of convolution, up-convoultion, pooling, and attention. Here we try to add a combination of spectral attention and spatial attention modules (SSAM) in each UNet layer. In detail, you can see the following figure:

![SSUNet_seaweed_new_upfont](https://github.com/user-attachments/assets/bcf74da8-00c5-48b0-95a1-d959a873b52a)

The model was built using remote sensing data, namely PlanetScope imagery. Several preprocessing treatments were applied to the dataset prior to label data generation. The label collection process applies the [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything).

The training model results show good accuracy. The inference model can be shown as follows. There are still some prediction results that show false negative and false positive. 
![compare](https://github.com/user-attachments/assets/e0229dc7-7321-487a-9698-9d5f367d6a19)
<img src="https://user-images.githubusercontent.com/116891235/396021378-e0229dc7-7321-487a-9698-9d5f367d6a19.png" width=50% height=50%>
