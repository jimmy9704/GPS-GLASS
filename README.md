# GPS-GLASS: Learning Nighttime Semantic Segmentation Using Daytime Video and GPS data
Official implementation of GPS-GLASS: Learning Nighttime Semantic Segmentation Using Daytime Video and GPS data [arXiv](https://arxiv.org/abs/2207.13297)

#####  Overview:
<img src="https://github.com/jimmy9704/GPS-GLASS/blob/main/image/network.png" width="800"/>

##### visualization results:
ACDC-night            |  Dark Zurich-val
:-------------------------:|:-------------------------:
<img src="https://github.com/jimmy9704/GPS-GLASS/blob/main/video/ACDC-night.gif" width="350"/> |<img src="https://github.com/jimmy9704/GPS-GLASS/blob/main/video/Dark_Zurich-val.gif" width="350"/>

## Web demo
[Here](https://8ce7-163-152-183-111.jp.ngrok.io/) you can upload your own image or select an example image to perform nighttime semantic segmentation using GPS-GLASS.

## Requirements
* python3.7
* pytorch==1.9.0
* cuda10.2

## Datasets
**Cityscapes**: Please follow the instructions in [Cityscape](https://www.cityscapes-dataset.com/) to download the training set.

**Dark-Zurich**: Please follow the instructions in [Dark-Zurich](https://www.trace.ethz.ch/publications/2019/GCMA_UIoU/) to download the training/val/test set.

**ACDC**: Please follow the instructions in [ACDC](https://acdc.vision.ee.ethz.ch/) to download the training/val/test set.

**NightCity+**: Please follow the instructions in [NightCity+](https://github.com/xdeng7/NightLab) to download the training/val set.

## Testing
Pretrained models can be downloaded form [here](https://www.dropbox.com/s/xmon1vnqsn2zvwz/trained_models.zip?dl=0).


To reproduce the reported results in our paper, follow these steps:
```
Step1: download the trained models and put it in the root.
Step2: change the data and model paths in configs/test_config.py
Step3: run "python evaluate.py"
Step4: change the ground truth data path in compute_iou.py
Step5: run "python compute_iou.py"
```
## Training 
Training code will be available upon acceptance of our manuscript.

## Acknowledgments
The code is based on [DANNet](https://github.com/W-zx-Y/DANNet), [AdaptSegNet](https://github.com/wasidennis/AdaptSegNet) .

## Related works
* [MGCDA](https://github.com/sakaridis/MGCDA)
* [GCMA](https://www.trace.ethz.ch/publications/2019/GCMA_UIoU/GCMA_UIoU-Sakaridis+Dai+Van_Gool-ICCV_19.pdf)
* [DANNet](https://github.com/W-zx-Y/DANNet)

## Citation
```
@article{lee2022gps,
  title={GPS-GLASS: Learning Nighttime Semantic Segmentation Using Daytime Video and GPS data},
  author={Lee, Hongjae and Han, Changwoo and Jung, Seung-Won},
  journal={arXiv e-prints},
  pages={arXiv--2207},
  year={2022}
}
```
