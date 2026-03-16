# Annotation Guidelines

## Annotation Format

All images in this dataset are annotated using the YOLO object detection format.

Each annotation file corresponds to one image and contains one or more bounding boxes.

The format of each annotation line is:

class_id x_center y_center width height

All values are normalized between 0 and 1 relative to image width and height.

## Class Definitions

The dataset uses the following class labels:

0 pothole
1 thela
2 animal
3 barricade
4 rickshaw

## Bounding Box Rules

During annotation the following rules were applied:

1. Bounding boxes should tightly cover the object.
2. Each object instance must have a separate bounding box.
3. Objects that are partially visible are annotated if at least 30 percent of the object is visible.
4. Extremely small objects that cannot be clearly identified are ignored.
5. Only the five predefined classes are annotated.

## Consistency

To maintain consistency across the dataset:

* similar object types are labeled using the same class
* overlapping objects are annotated individually
* ambiguous objects are excluded from annotation

These rules help ensure reliable training data for object detection models.
