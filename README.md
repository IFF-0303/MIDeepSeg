## MIDeepSeg
This repository proivdes a 2D medical image interactive segmentation method for segmentation and annotation.
 ![image](https://github.com/Luoxd1996/MIDeepSeg/blob/master/demo_video/demo.gif)

## Requirements
Before you can use this package for image segmentation. You should:
* [Pytorch][torch_link] version >=1.0.1
* Some common python packages such as Numpy, Pandas, SimpleITK,OpenCV
* Install the [geodesic_distance_tool][geos_dis_link] for geodesic distance transformation.
* Install the [SimpleCRF][simplecrf_link] for interactive refinement.

[geos_dis_link]: https://github.com/taigw/GeodisITK
[simplecrf_link]: https://github.com/HiLab-git/SimpleCRF
## How to use
1. launch the GUI
```bash
python mideepseg/main.py
``` 
2. load an image for segmentation. Once the image is loaded,  Firstly, give some edge points by left mouse to get an initial interactions, click the Segmentation button to obtain an initial segmentation. Then, press left mouse button to give clicks in under-segmented regions, and press right mouse button to give clicks  in over-segmented region. Then click the Refinement button, and the segmentation will be updated according to the interactions.

3. Note that, the pretrained model is only trained with placenta, fetal brain in T2-MRI and liver in CT.
