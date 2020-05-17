# ImageSegmentation

The repository contains three different models for image segmentation

1. Pretrained DeepLabv3+ on Pascal Voc
2. Unet for medical data 
3. Rnn for segmenting images based on their description

Each model requires different imports and versions:


| DeepLabv3+        | UNet            | RNN |
|-------------------|-----------------|-----|
| tensorflow==1.x   | tensorflow==2.x |     |
| matplotlib        | matplotlib      |     |
| pillow            | pillow          |     |
| os                | os              |     |
|                   | keras_unet      |     |
|                   | glob            |     |
|                   | sklearn         |     |



**DeepLabv3+**

The code includes a pretrained model with two different backbones (mobilenetv2 and xception). It was trained on the Pascal Voc dataset and therefore only detects its included classes. However, you can provide any image input via its corresponding url.

**UNet:**



**Custom data**

If you plan on preparing you own dataset for training, this pixel annotation tool might be helpful:
https://github.com/abreheret/PixelAnnotationTool

