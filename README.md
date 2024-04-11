# GeneralizedPanopticQuality

Repository for the paper "A sharper definition of alignment for Panoptic Quality" currently under review at the Pattern Recognition Letters journal

## Code structure



## Setup

As this work is about comparing the output of a well-performing instance segmentation model on three different datasets, we take models finetuned on these
three datasets from the (Detectron2 Model Zoo)[https://github.com/facebookresearch/detectron2/blob/main/MODEL_ZOO.md] and performed inference on the test/val portions of these three datasets. `XXX` contains the script to download
the datasets and models, and `XXX` contains the scripts required to run the trained models on the test/val sets of the three datasets. We used standard scripts from 
Detectron2 for the inference. The CityScapes datasset has to be downloaded seperately from [the website](https://www.cityscapes-dataset.com) and an account is required to download the data.

All the datasets used in this research are publicly available and can be downloaded via the respective websites.
We have also included download scripts for each of the individual datasets, as especially the COCO dataset is quite large, and
downloading it might take up quite some space.
