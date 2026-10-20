# RBC Blood Cells

RBC blood cell object detection project.

## Dataset Structure

RBC_Blood_Cells/
├── images/
├── Images_With_Boxes/
├── train/
│   ├── images/
│   └── labels/
├── val/
│   ├── images/
│   └── labels/
├── test/
│   ├── images/
│   └── labels/
├── data.yaml
├── FINAL_REPORT.md
└── README.md

The images/ folder contains the complete collection of 586 clean images.

## Annotation Format

YOLO Object Detection format:

Class X_center Y_center Width Height

All coordinates are normalized between 0 and 1.

Each image is paired with the annotation file using the same number.

## Dataset Split

Train: 410 images (70%)
Validation: 117 images (20%)
Test: 59 images (10%)

The split is class-aware and performed at the image level.

The image and its corresponding annotation always remain together.

## Classes

The final dataset contains 12 RBC classes:

0 = Normal cell
1 = Macrocyte
2 = Microcyte
3 = Spherocyte
4 = Target cell
5 = Stomatocyte
6 = Ovalocyte
7 = Teardrop
8 = Burr cell
9 = Schistocyte
10 = uncategorised
11 = Hypochromia

## Dataset and Data Engineering Pipeline

### 1. Dataset Source

The original **Chula-RBC-12** dataset was provided by the **Chula PIC Lab** and was used as the source dataset for this project.

### 2. My Custom Data Engineering Pipeline

I independently processed and prepared the dataset for object detection. The custom data engineering pipeline included:

* Extracting the **cell center coordinates** from the original annotations.
* Generating bounding-box dimensions (**Width (W)** and **Height (H)**) from the original cell-box information.
* Converting the bounding-box annotations into the standard **YOLO normalized format** (`Class, X_center, Y_center, W, H`), with coordinates normalized relative to the image dimensions.
* Verifying and organizing the final collection of **586 clean images**.
* Matching each clean image with its corresponding annotation file.
* Structuring the prepared images and corresponding annotation files into dedicated **train**, **val**, and **test** directories.
* Applying a **class-aware split** while preserving each image and its complete annotation set as one unit.
* Creating a complete `images/` directory containing all 586 clean images.
* Creating the `data.yaml` configuration file required for YOLO training.
* Creating a structured, reproducible dataset package suitable for an **Object Detection** pipeline.

## Data Configuration

The final dataset contains 12 classes numbered 0 through 11.

Class 12 was removed from the final configuration.