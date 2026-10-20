# Plasmodium falciparum Object Detection

## Goal
Single-class object detection using YOLO.

## Class
- Class ID: 0
- Class name: falciparum

## Folder structure
- 01_original_dataset_images/: all original images without boxes.
- 02_falciparum_images_with_boxes/: separate display copies with boxes.
- train/images/: original training images without drawn boxes.
- train/labels/: YOLO training annotations.
- val/images/: original validation images without drawn boxes.
- val/labels/: YOLO validation annotations.
- test/images/: original test images without drawn boxes.
- test/labels/: YOLO test annotations.
- data.yaml: YOLO dataset configuration.
- classes.txt: class names.

## Counts
Original images copied: 210
Images in train/val/test: 209
Images with Falciparum boxes: 103
Images without recorded Falciparum boxes: 106
Total Falciparum boxes: 1267
Images rendered with boxes: 103

## Split details

- train: 134 images, 67 images with boxes, 67 images without recorded boxes, 516 boxes.
- val: 35 images, 20 images with boxes, 15 images without recorded boxes, 353 boxes.
- test: 40 images, 16 images with boxes, 24 images without recorded boxes, 398 boxes.

## Annotation notes
The YOLO boxes were derived from bitmap masks in the prepared dataset.
Images with drawn boxes are separate display copies. The original images
and train/val/test images are not modified.

An empty label means no Falciparum box is recorded for that image.
It does not prove that the image contains healthy blood. Images
containing other Plasmodium species must not be described as confirmed
normal-blood samples.

Review annotations visually before training or drawing medical conclusions.

## Source
MP-IDB dataset downloaded through DatasetNinja.
Retain the original attribution and licensing terms when redistributing.
