# GeneralizedPanopticQuality

Repository for the paper "A sharper definition of alignment for Panoptic Quality" currently under review at the Pattern Recognition Letters journal.

This repository contains the code used to conduct the experiments in the paper, as well as the config files that were used to evaluate the models on the COCO, LVIS and CityScapes datasets.

## Code structure
- The main code is stored in the `notebooks` folder, with the `InstanceSegmentationExperiments.ipynb` notebook containing the comparison between the two different matchings.
- The `config` directory stores the config files that were used to run the evaluation scripts from the Detectron2 library with the appropriate models.
- The `results` folder contains the raw outputs of the model on the different datasets, in the COCO annotation format.
- The `pq_results` folder contains the scores for all three datasets calculated with both matchings of the PQ algorithm.



## Setup

As this work is about comparing the output of a well-performing instance segmentation model on three different datasets, we take models finetuned on these
three datasets from the (Detectron2 Model Zoo)[https://github.com/facebookresearch/detectron2/blob/main/MODEL_ZOO.md] and performed inference on the test/val portions of these three datasets.
We used standard scripts from Detectron2 for the inference. The CityScapes dataset has to be downloaded seperately from [the website](https://www.cityscapes-dataset.com) and an account is required to download the data.
