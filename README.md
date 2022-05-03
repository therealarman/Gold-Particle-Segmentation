
# 🔬 Gold Particle Detection 🧠

## Overview
This project makes use of the [**YoloV5**](https://github.com/ultralytics/yolov5) model architecture for the detection and labeling of Immunogold Particles.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/therealarman/Gold-Particle-Segmentation/blob/main/YOLOv5_Gold_Particle.ipynb]

2 different datasets were used in the training of this project.
1. Roboflow annotated images w rotation & flipped axis augmentation (Downsized and cropped to 416x416)
2. Provided data with no data augmentation (Downsized and cropped to 512x512)

The first dataset contained only 6nm particle data, while the second contained both 6nm and 12nm particle data.
The results for each are shown below.
## Results

### First Training
>*27 Training Images (Augmented Data from Roboflow)*
>*1000 Epochs*
>*1 class (6 nm Particles)*

![TensorBoard](https://raw.githubusercontent.com/therealarman/Gold-Particle-Segmentation/main/img/GoldParticleMetrics.PNG)

| mAP_0.5 | Percision | Recall |
|  :---:  |   :----:  | :---:  |
|  0.789  |   0.827   | 0.755  |
|  78.9%  |   82.7%   | 75.5%  |

*Example 1:*
![Example1](https://raw.githubusercontent.com/therealarman/Gold-Particle-Segmentation/main/img/S1%20MBTt4%20FFRIL%208wks%20Wt2%20R5Ag19a%20vGlut%2018nm_panAMPA%2012nm_NR1_6nm__0003.tif.jpg)
*Example 2:*
![Example2](https://raw.githubusercontent.com/therealarman/Gold-Particle-Segmentation/main/img/S24%20MBTt4%20FFRIL%208wks%20Het1%20R4Bg18e%20vGlut%2018nm_panAMPA%2012nm_NR1_6nm__0003.tif.jpg)
*Example 3:*
![Example3](https://raw.githubusercontent.com/therealarman/Gold-Particle-Segmentation/main/img/S29%20MBTt4%20FFRIL%208wks%20Wt2%20R5Ag19a%20vGlut%2018nm_panAMPA%2012nm_NR1_6nm__0004.tif.jpg)
*Example 4:*
![Example4](https://raw.githubusercontent.com/therealarman/Gold-Particle-Segmentation/main/img/S31%20MBTt4%20FFRIL%208wks%20Het1%20R4Bg18e%20vGlut%2018nm_panAMPA%2012nm_NR1_6nm__0003.tif.jpg)

### Second Training
>*9 Images (Cropped and Downsized to 512x512)*
>*1000 Epochs*
>*2 classes (6 nm & 12 nm)*

![TensorBoard](https://raw.githubusercontent.com/therealarman/Gold-Particle-Segmentation/main/img/GoldParticleTrain2.png)

| mAP_0.5 | Percision | Recall |
|  :---:  |   :----:  | :---:  |
|  0.791  |   0.642   | 0.87  |
|  79.1%  |   64.2%   | 87.5%  |

*Example 1:*
![Example1](https://raw.githubusercontent.com/therealarman/Gold-Particle-Segmentation/main/img/S1%20MBTt4%20FFRIL%208wks%20Wt2%20R5Ag19a%20vGlut%2018nm_panAMPA%2012nm_NR1_6nm__0003.jpg)
*Example 2:*
![Example2](https://raw.githubusercontent.com/therealarman/Gold-Particle-Segmentation/main/img/S31%20MBTt4%20FFRIL%208wks%20Het1%20R4Bg18e%20vGlut%2018nm_panAMPA%2012nm_NR1_6nm__0003.jpg)
*Example 3:*
![Example3](https://raw.githubusercontent.com/therealarman/Gold-Particle-Segmentation/main/img/E3%20MBTt4%20FFRIL%208wks%20Het1%20R4Bg18e%20vGlut%2018nm_panAMPA%2012nm_NR1_6nm__0004.jpg)
*Example 4:*
![Example4](https://raw.githubusercontent.com/therealarman/Gold-Particle-Segmentation/main/img/D1%20MBTt4%20FFRIL%208wks%20Wt2%20R5Ag19a%20vGlut%2018nm_panAMPA%2012nm_NR1_6nm__0003.jpg)