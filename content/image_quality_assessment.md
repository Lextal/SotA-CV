# Image Quality Assessment

## Description
Image quality (often Image Quality Assessment, IQA) is a characteristic of an image that measures the perceived image degradation (typically, compared to an ideal or perfect image). In computer vision, it may compare resolution, blurring ,noise etc, and  use regression/classification to give a judgement.

Usual evaluation metrics are:

* Linear Correlation Coefficient(LCC): LCC is a measure of the linear correlation between the
ground truth and the predicted quality scores
* Spearman Rank Order Correlation Coefficient (SROCC): The SROCC measures the monotonic
relationship between ground-truth and estimation

*refer here(https://arxiv.org/pdf/1707.08347.pdf)


## Results


### LIVE — Testing set

[Dataset description](datasets/pascal_voc_2012_segmentation.md)

| Model | LCC | SROCC | Weights | Paper | Code |
|:------|:-----|:-----|:--------|:------|:-----|
| VGG-16                | 0.973 | 0.974 |  [model](https://github.com/xialeiliu/RankIQA/blob/master/pre-trained)|[paper](https://arxiv.org/pdf/1707.08347.pdf) | [Caffe](https://github.com/xialeiliu/RankIQA) |


### TID 2013 — Testing set

[Dataset description](datasets/pascal_voc_2012_segmentation.md)

| Model | LCC | SROCC | Weights | Paper | Code |
|:------|:-----|:-----|:--------|:------|:-----|
| VGG-16                | NA | 0.780 |  [model](https://github.com/xialeiliu/RankIQA/blob/master/pre-trained)|[paper](https://arxiv.org/pdf/1707.08347.pdf) | [Caffe](https://github.com/xialeiliu/RankIQA) |
