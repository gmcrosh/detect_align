# Detect Align

MTCNN approach to face detection can be slower (if not tuned) for larger images, while an SSD approach is fast but doesn't align images. By combining an SSD and the Onet of MTCNN you can quickly detect faces and align them.

## Onet
The final network in the MTCCN approach. Returns bounding box refinement, anchors, and probability.

## SSD
Uses ssd_mobilenet_v1_coco_2018_01_28 retrained on WIDERFACE, requires Tensorflow Object Detection to be installed ([instructions](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/installation.md))