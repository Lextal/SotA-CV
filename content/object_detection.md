# Object detection

## Description

This task encompasses both finding spatial location
of an entity and assigning a class label to the located object.
The goal is to produce bounding boxes with corresponding classes for an input image.

Two main metrics are mean Average Precision (mAP) and mean Average Recall (mAR).
They are used in the same way as with multi-class classification problem
with two additional constraints:

1. Predicted bounding box must be close enough to the ground truth box.
2. The probability of a class must be greater than a fixed threshold.

## Results

### MS-COCO

[Dataset description](datasets/...)

| Model | Score | Weights | Paper | Code |
|:------|:-----:|:--------|:------|:-----|
| Model name | 0.5 | [link to the weights of a trained model]() | [paper](https://arxiv.org/abs/0000.00000) | [link to implementation]() |

### PASCAL VOC 2012

[Dataset description](datasets/...)

| Model | Score | Weights | Paper | Code |
|:------|:-----:|:--------|:------|:-----|
| Model name | 0.5 | [link to the weights of a trained model]() | [paper](https://arxiv.org/abs/0000.00000) | [link to implementation]() |

### Resources
