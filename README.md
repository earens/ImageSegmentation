# Image Segmentation

The repository contains two different models for image segmentation

1. Pretrained DeepLabv3+ on Pascal Voc
2. Unet for medical data 

Each model requires different imports and versions:


| DeepLabv3+        | UNet            | 
|-------------------|-----------------|
| tensorflow==1.x   | tensorflow==2.x |     
| matplotlib        | matplotlib      |     
| pillow            | pillow          |     
| os                | os              |     
|                   | keras_unet      |     
|                   | glob            |     
|                   | sklearn         |  



**DeepLabv3+**

The code includes a pretrained model with two different backbones (mobilenetv2 and xception). It was trained on the Pascal Voc dataset and therefore only detects its included classes. However, you can provide any image input via its corresponding url.

**UNet:**

The code includes a unet which performs image segemnentation for masks with n numbers of classes. This code loads a medical dataset with one class only. If you want to try a dataset with different amounts of classes you have to adapt the plot function.


**Custom data**

If you plan on preparing you own dataset for training, this pixel annotation tool might be helpful:
https://github.com/abreheret/PixelAnnotationTool

Sarah, Emilia
