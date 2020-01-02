# Unknown Identity Rejection Loss: selected code

We release part of our experimental code as a reference for readers that are interested in our paper: [Unknown Identity Rejection Loss: Utilizing Unlabeled Data for Face Recognition](https://arxiv.org/abs/1910.10896)

## Introduction

We proposed the Unseen Identity Rejection Loss to utilize the unlabeled data for training discriminative feature representations for face recognition. By introducing features of unknown faces into the high-dimensional space, the feature space can be rearranged so that margins between samples can be further optimized. 

![](https://github.com/HoiM/UIR-Loss-selected-code/blob/master/images/picture.png)

## Selected results

Below is the performance of our trained ResNet-100 model on the IJB-C dataset.

![](https://github.com/HoiM/UIR-Loss-selected-code/blob/master/images/table.png)

## Selected code

The implementation of the loss function is in lines 252~265 of ```selelcted_code/semisupervised-finetune.py```. Our implementation is based on the [InsightFace](https://github.com/deepinsight/insightface) repository. Here we used ResNet-100 as the backbone network and arcface loss function for supervised training. 

## Citation

If you find our method useful in your research, please consider citing the following related paper.

```latex
@article{uirloss,
  title={Unknown Identity Rejection Loss: Utilizing Unlabeled Data for Face Recognition},
  author={H. Yu and Y. Fan and K. Chen and Y. He and X. Lu and J. Liu and D. Xie},
  journal={ICCV Workshop},
  year={2019}
}
```
