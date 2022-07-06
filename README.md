# GPS-GLASS: Learning Nighttime Semantic Segmentation Using Daytime Video and GPS data

##### visualization results:
ACDC-night            |  Dark Zurich-val
:-------------------------:|:-------------------------:
<img src="https://github.com/jimmy9704/GPS-GLASS/blob/main/video/ACDC-night.gif" width="500"/> |<img src="https://github.com/jimmy9704/GPS-GLASS/blob/main/video/Dark_Zurich-val.gif" width="500"/>

## Requirements
* python3.7
* pytorch==1.9.0
* cuda10.2

## Datasets
**Cityscapes**: Please follow the instructions in [Cityscape](https://www.cityscapes-dataset.com/) to download the training set.

**Dark-Zurich**: Please follow the instructions in [Dark-Zurich](https://www.trace.ethz.ch/publications/2019/GCMA_UIoU/) to download the training/val/test set.

**ACDC**: Please follow the instructions in [ACDC](https://acdc.vision.ee.ethz.ch/) to download the training/val/test set.

**NightCity+**: Please follow the instructions in [NightCity+](https://github.com/xdeng7/NightLab) to download the training/val/ set.

## Testing
To reproduce the reported results in our paper, follow these steps:
```
Step1: download the [trained models](https://www.dropbox.com/s/16dw0h0oz5u70e2/trained_models.zip?dl=0) and put it in the root.
Step2: change the data and model paths in configs/test_config.py
Step3: run "python evaluation.py"
Step4: run "python compute_iou.py"
```
## Training 
Training code will be available upon acceptance of our manuscript.

## Acknowledgments
The code is based on [DANNet](https://github.com/W-zx-Y/DANNet), [AdaptSegNet](https://github.com/wasidennis/AdaptSegNet) .

## Related works
* [MGCDA](https://github.com/sakaridis/MGCDA)
* [GCMA](https://www.trace.ethz.ch/publications/2019/GCMA_UIoU/GCMA_UIoU-Sakaridis+Dai+Van_Gool-ICCV_19.pdf)
* [DANNet](https://github.com/W-zx-Y/DANNet)
