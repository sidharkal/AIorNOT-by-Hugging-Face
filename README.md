# AIorNOT-From-Hugging-Face

In this competition, your task is to build a model that can identify ai generated images.

![This is an image](https://huggingface.co/spaces/competitions/aiornot/resolve/main/comp.png)

## Overview
The dataset consists of approximately 31000 images, some of which have been generated by ai. Your task is to build a model that can identify ai generated images. Please use the community tab for discussion and questions.

## Submission format and evaluation metric
The evaluation metric for this competition is logloss. The submission file should be a csv file with the following format:

```
id,        label
0.jpg,     0.1
1.jpg,     0.5
10.jpg,    0.8
100.jpg,   0.9
1000.jpg,  0.2
10000.jpg, 0.4
10001.jpg, 0.3
```

Logloss metric is the same as available in scikit-learn. You can use the following code to calculate the logloss:

```
from sklearn.metrics import log_loss
log_loss(y_true, y_pred)
```
