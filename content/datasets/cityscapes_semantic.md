# Cityscapes — Semantic Segmentation

### Description

* [The Cityscapes Dataset for Semantic Urban Scene Understanding](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Cordts_The_Cityscapes_Dataset_CVPR_2016_paper.pdf)
* [Official website](https://www.cityscapes-dataset.com/)

The access to archive with the dataset and the evaluation endpoint are
both located at [the website of the challenge](https://www.cityscapes-dataset.com/).

The performance of a segmentation model is evaluated using class-mIoU, category-mIoU, instance mIoU and pixel accuracy.


### Technical details

* Train/validation/test sets are split into separate sets
of 2975, 500, and 1525 images respectively.
* The size of each image is 1024x2048.
* The dataset contains 19 object classes and additional instance-level labeling.


### Format

Train and validation sets contain input RGB images supplemented by
labels in separate files organized in the following way:

Each folder contains images separated by scene category (same scene categories than the Places Database). For each image, the object and part segmentations are stored in two different png files. All object and part instances are annotated sparately.

For each image there are the following files:

##### \*_leftImg8bit.png

Input RGB image.

##### \*_gtFine_labelIds.png

RGB image with object segmentation mask. Each pixel is represented by
a single-byte unsigned integer that indicates the correct class label.
Some classes should be ignored during training.

### Tools

Links to helper scripts for extraction/transformation/visualization.

| Link | Description |
|:-----|:------------|
| [Cityscapes Scripts](https://github.com/mcordts/cityscapesScripts) | A collection of scripts for inspection, preparation, and evaluation. |
