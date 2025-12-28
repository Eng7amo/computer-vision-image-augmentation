# Image Augmentation Pipeline for Wildlife Detection

## Objective
The goal of this project is to design an image processing pipeline that augments wildlife images to improve the robustness of object detection models.

The pipeline performs controlled transformations on a limited set of images to generate diverse training samples.

---

## Dataset
Images are sourced from the COCO (Common Objects in Context) dataset and feature various animals in natural environments.

Input images:
- 000000546829.jpg
- 000000012062.jpg
- 000000417085.jpg
- 000000269314.jpg
- 000000575357.jpg

---

## Methodology

### Image Processing Steps
1. **Image Import**
   - Load images using `skimage.io.imread`

2. **Resizing**
   - Normalize image dimensions to a fixed resolution

3. **Rotation**
   - Apply controlled angular rotations to simulate viewpoint changes

4. **Contrast Enhancement**
   - Use adaptive histogram equalization (CLAHE) to improve feature visibility

---

## Implementation
The pipeline is implemented as a reusable Python function that:
- Accepts multiple images
- Applies configurable transformations
- Returns augmented images for downstream tasks

---

## Tools Used
- scikit-image (resize, rotate, equalize_adapthist)
- Matplotlib (visualization)

---

## Output
- Augmented image dataset
- Side-by-side visualization of transformed images
- Reusable preprocessing pipeline for computer vision workflows

---

## Notes
This project focuses on preprocessing and data preparation, which are critical steps in successful computer vision systems.

