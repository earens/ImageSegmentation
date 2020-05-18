# Image Segmentation

The repository contains two different models for image segmentation

1. Pretrained DeepLabv3+ on Pascal Voc
2. Unet for medical data 

As well as code for a webcam application:

3. DeepLabv3+ on Pascal Voc for webcam data

Each model requires different imports and versions:


| DeepLabv3+        | UNet            | DeepLabv3+ Webcam|
|-------------------|-----------------|------------------|
| tensorflow==1.x   | tensorflow==2.x | tensorflow==1.x  | 
| matplotlib        | matplotlib      | matplotlib       |
| pillow            | pillow          | pillow           |
| os                | os              | os               |    
|                   | keras_unet      | open CV          |    
|                   | glob            |                  | 
|                   | sklearn         |                  | 



**DeepLabv3+**

The code includes a pretrained model with two different backbones (mobilenetv2 and xception). It was trained on the Pascal Voc dataset and therefore only detects its included classes. However, you can provide any image input via its corresponding url.

https://github.com/tensorflow/models/blob/master/research/deeplab/deeplab_demo.ipynb

**UNet:**

The code includes a unet which performs image segemnentation for masks with n numbers of classes. This code loads a medical dataset with one class only. If you want to try a dataset with different amounts of classes you have to adapt the plot function.


**DeepLabv3+ WebCam**

Apart from the common application on the Pascal Voc dataset, this code offers image segmentation of webcam data. In order to run it you need to keep the utils folder (tensorflow/models/tree/master/research/deeplab) which is already included in this repository, in the same folder as the webcam code. 
The model is pretrained on Pascal Voc and therefore only recognizes the classes belonging to this dataset. Sadly the frame rate is really low and we did not yet find a solution for this problem. However, it might still be interesting as it contains an attempt for real time segmentation.

https://www.novatec-gmbh.de/blog/semantic-segmentation-part-1-deeplab-v3/



**Custom data**

If you plan on preparing you own dataset for training, this pixel annotation tool might be helpful:
https://github.com/abreheret/PixelAnnotationTool

Sarah, Emilia
