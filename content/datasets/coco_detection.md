# COCO Dataset 2016 — Detection

### Description



* [Microsoft COCO: Common Objects in Context](https://arxiv.org/abs/1405.0312)
* [Common Objects in Context](http://cocodataset.org)

The challenge uses several metrics, but among typically reported are:

* **Mean Average Precision**
* **Average Precision @ 0.5, 0.75 IoU** for labels on bounding boxes having >= 0.5 IoU with ground truth — primary metric.
* **AP-small** — AP for instances with areas (total pixels) < 1024
* **AP-medium** — AP for instances with 1024 <= area < 9216
* **AP-large** — AP for instances with area >= 9216

### Downloads

* [Train images](http://images.cocodataset.org/zips/train2014.zip)
* [Validation images](http://images.cocodataset.org/zips/val2014.zip)
* [Train/val annotations](http://images.cocodataset.org/annotations/annotations_trainval2014.zip)
* [Test images](http://images.cocodataset.org/zips/test2015.zip)
* [Test images info](http://images.cocodataset.org/annotations/image_info_test2015.zip)


### Technical details

* Train set: ~83000 images, 604907 instances
* Validation set: ~41000 images
* 80 classes joined into 12 supercategories
* Number of pixels: 90% of images have between 167500 and 355840 pixels in train set.
* Height/width ratio: 90% of images have the ration between 0.6 and 1.5 in train set.
* Number of instances: 99% of images contain between 1 and 33 different instances, median = 4 (train set).


### Format

Target labeling in contained in separate JSON files.
Bounding boxes and corresponding labels are provided in `instances_train2014.json` and `instances_val2014.json`.

Instance annotations are stored in lists under the `annotations` key in corresponding files.
Each object contains an annotation of one instance in one image.
For the detection task the following fields are of particular interest:

* `image_id`: ID of the input image in the database
* `bbox`: 4-tuple containing the keypoint of a rectangular bounding box
* `category_id`: number of class associated with the instance

Information about categories, such as names and ids can be found under the key `categories`.
Information about images (file name, resolution, id, area) can be found under the key `images`.

The maintainers of the dataset provide a multi-language API (listed below) for handling the index for the entire database.

### Resources

Links to helper scripts for extraction/transformation/visualization.

| Link | Description |
|:-----|:------------|
| [COCO API](https://github.com/cocodataset/cocoapi) | Lua, Matlab, and Python APIs for handling COCO dataset. |

### Demo
