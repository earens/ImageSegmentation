# ImageSegmentation

The repository contains three different models for image segmentation

1. Pretrained DeepLabv3+ on Pascal Voc
2. Unet for medical data 
3. Rnn for segmenting images based on their description

Each model requires different imports and versions:

1. DeepLabv3+:
  * tensorflow==1.x
  * matplotlib
  * pillow
  * os

2. UNet:
  * tensorflow==2.x
  * keras_unet
  * matplotlib
  * glob
  * os
  * pillow
  * sklearn
  
3. RNN:



**DeepLabv3+**

The code includes a pretrained model with two different backbones (mobilenetv2 and xception). It was trained on the Pascal Voc dataset and therefore only detects its included classes. However, you can provide any image input via its corresponding url.

**UNet:**



**Custom data**

If you plan on preparing you own dataset for training, this pixel annotation tool might be helpful:
https://github.com/abreheret/PixelAnnotationTool

