# Image Quality Assessment

## Description
Image quality (often Image Quality Assessment, IQA) is a characteristic of an image that measures the perceived image degradation (typically, compared to an ideal or perfect image). In computer vision, it may compare resolution, blurring ,noise etc, and  use regression/classification to give a judgement.

Usual evaluation metrics are:

* Linear Correlation Coefficient(LCC): LCC is a measure of the linear correlation between the
ground truth and the predicted quality scores
* Spearman Rank Order Correlation Coefficient (SROCC): The SROCC measures the monotonic
relationship between ground-truth and estimation

*refer here(https://arxiv.org/abs/1707.08347)


## Results


### LIVE — Testing set


| Model | LCC | SROCC | Weights | Paper | Code |
|:------|:-----|:-----|:--------|:------|:-----|
| VGG-16                | 0.973 | 0.974 |  [Caffe](https://github.com/xialeiliu/RankIQA/blob/master/pre-trained)|[paper](https://arxiv.org/abs/1707.08347) | [Caffe](https://github.com/xialeiliu/RankIQA) |


### TID 2013 — Testing set


| Model | LCC | SROCC | Weights | Paper | Code |
|:------|:-----|:-----|:--------|:------|:-----|
| VGG-16                | N/A | 0.780 |  [Caffe](https://github.com/xialeiliu/RankIQA/blob/master/pre-trained)|[paper](https://arxiv.org/abs/1707.08347) | [Caffe](https://github.com/xialeiliu/RankIQA) |
