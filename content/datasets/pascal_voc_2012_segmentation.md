# PASCAL VOC 2012 — Segmentation

### Description

* [Paper](https://link.springer.com/content/pdf/10.1007/s11263-009-0275-4.pdf)
* [Website](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/htmldoc/devkit_doc.html#SECTION00060000000000000000)
* [Evaluation server (registration required)](http://host.robots.ox.ac.uk:8080/)

RGB images with corresponding pixel-wise annotations.
Images are containing realistic everyday scenes.

For evaluation the usual metric is mean Intersection over Union (mIoU).

### Downloads

* [Train and validation sets](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/VOCtrainval_11-May-2012.tar)

### Technical details

Available data is split into **train** and **val** sets,
containing 1464 and 1449 images respectively.

* 20 class labels + background + unlabeled
* Median number of pixels: 187500, 90% of images have between 147000 and 200000 pixels
* Median height-to-width ratio is 0.75, 90% of images have between 0.66 and 1.5.

### Resources

Links to helper scripts for extraction/transformation/visualization.

| Link | Description |
|:-----|:------------|
| [Dataset scripts](https://github.com/warmspringwinds/tf-image-segmentation/blob/master/tf_image_segmentation/utils/pascal_voc.py) | A collection of utility functions in Python |

### Demo
