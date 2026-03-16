# Labeling Examples

This document provides examples of how objects are annotated in the dataset.

## Example Image

Image file:

img_0123.jpg

Corresponding annotation file:

img_0123.txt

Annotation contents:

1 0.532 0.417 0.210 0.265

## Interpretation

class_id: 1
class_name: thela

Bounding box center:

x_center: 0.532
y_center: 0.417

Bounding box size:

width: 0.210
height: 0.265

All coordinates are normalized values between 0 and 1.

## Multiple Objects Example

If an image contains multiple objects, the annotation file will contain multiple lines.

Example:

0 0.445 0.621 0.190 0.150
4 0.630 0.540 0.300 0.310

This means:

* a pothole detected at the first location
* a rickshaw detected at the second location

Each object instance is recorded separately.

## Annotation Workflow

The labeling process typically follows these steps:

1. open the image in the annotation tool
2. draw a bounding box around the object
3. assign the correct class label
4. save the annotation in YOLO format

This process is repeated for all objects present in the image.
