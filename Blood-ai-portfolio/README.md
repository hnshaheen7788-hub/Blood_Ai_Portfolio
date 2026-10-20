# Hend Shaheen | Medical AI Portfolio

**Medical Laboratory Technician · Medical Image Annotation · Medical AI / Computer Vision**

I am a medical laboratory technician with a background in hematology and malaria microscopy. I am developing practical skills in medical-image data preparation, bounding-box annotation, label review, and computer-vision workflows. My current portfolio focuses on blood-cell and malaria-related image datasets.

My goal is to combine my laboratory background with technical skills to contribute to entry-level projects in **medical image annotation, dataset preparation, and medical AI/computer vision**.

## Background

- **Education:** Technical Health Institute, Tanta, Egypt — Medical Laboratory Technology, 2021
- **Laboratory experience:** Malaria microscopy, CBC/hematology, clinical chemistry, and routine stool and urine testing
- **Medical image knowledge:** Familiar with examining blood-cell morphology under a microscope and distinguishing normal from abnormal appearances within the limits of laboratory review

## Technical Skills

- **Programming:** Python fundamentals
- **Data-preparation environment:** Visual Studio Code (VS Code)
- **Image processing:** OpenCV
- **Numerical data:** NumPy
- **Annotation review interface:** Tkinter
- **Annotation workflow:** Bounding-box creation and correction, label-file preparation, visual/manual quality review
- **Model training and evaluation:** YOLO with Ultralytics; reading Precision, Recall, and mAP metrics
- **Notebook environments:** Kaggle Notebooks and Google Colab; used an NVIDIA Tesla T4 GPU for training experiments
- **Computer skills:** Microsoft Word and Microsoft Excel

I am continuing to build my programming and model-development skills. Some workflows were completed with code assistance, and I describe each project below according to the work completed.

## Projects

### 1. RBC Dataset Preparation and Annotation

**Status: Data preparation and review completed; no model training claimed for this project.**

- Prepared and reviewed a red-blood-cell image dataset with 12 categories supplied by the original dataset.
- Created and corrected bounding-box coordinates with code assistance, then manually and visually reviewed annotations.
- Organized image and label files into training, validation, and test splits and prepared a `data.yaml` file.

**Project files:** [RBC dataset project](./RBC_Dataset_Project/RBC_Blood_Cells/) · [Project README](./RBC_Dataset_Project/RBC_Blood_Cells/README.md) · [Final report](./RBC_Dataset_Project/RBC_Blood_Cells/FINAL_REPORT.md)

![RBC dataset overview](./Screenshots/RBC_Dataset.png)

![RBC annotation example](./Screenshots/RBC_Annotation.png)

### 2. Platelet Detection with YOLO

**Status: Data preparation and review completed; YOLO training performed.**

- Prepared and reviewed platelet images, labels, and bounding boxes.
- Ran YOLO training experiments with the Ultralytics library and reviewed training/evaluation outputs.
- Saved model and evaluation artifacts, including the `best.pt` checkpoint and available plots/reports.
- **Best recorded validation mAP@50: 97.95% at Epoch 34.** This is a validation result, not a result from an independent test set; it should not be interpreted as a test score.

**Project files:** [Platelet detection project](./Platelet_Detection_Project/) · [Model package and evaluation artifacts](./Platelet_Detection_Project/platelets_model_package/)

![Platelet detection results](./Screenshots/Platelet_Results.png)

### 3. *Plasmodium falciparum* Dataset Preparation

**Status: Data preparation and review completed; no trained malaria model is presented in this portfolio.**

- Prepared and reviewed malaria-related images, label files, box coordinates, and annotations.
- Organized the working dataset into training, validation, and test splits.
- Kept the project focused on dataset preparation and annotation quality rather than claiming a trained model.

The complete malaria dataset and model weights are not bundled with this portfolio at present.

![Malaria annotation example](./Screenshots/Malaria_Annotation.png)

## Annotation Quality Principles

Across my dataset projects, I focus on boxes that closely fit one target object, clear labels, review of box coordinates, and visual/manual checking. I also check for boxes cut off by image edges and other obvious annotation issues where relevant to the project.

## Current Learning Focus

- Improving Python programming and code-reading skills
- Strengthening medical-image annotation and dataset quality review
- Learning more about computer-vision model evaluation and reproducible experiments

## Notes

- The reported platelet result is a **validation metric** and is labeled accordingly.
- RBC and malaria projects are presented as data-preparation and annotation projects, not as completed model-training projects.
- This portfolio is for technical demonstration and learning; it is not a clinical diagnostic system.
