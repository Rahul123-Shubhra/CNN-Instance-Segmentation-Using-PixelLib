# CNN Instance Segmentation Using PixelLib

## Overview

This project implements **Instance Segmentation and Object Detection** using **PixelLib**, **Mask R-CNN**, and **TensorFlow**. The model is pre-trained on the **COCO dataset** and can identify multiple objects in an image while generating accurate segmentation masks and bounding boxes.

The application processes an input image, detects objects present in the scene, and produces an output image with segmented objects and labeled bounding boxes.

---

## Features

* Instance Segmentation using Mask R-CNN
* Object Detection with Bounding Boxes
* COCO Pretrained Model Support
* Automatic Object Classification
* Segmentation Mask Generation
* Image Processing and Visualization
* Deep Learning-based Computer Vision Pipeline

---

## Technologies Used

* Python
* TensorFlow
* PixelLib
* Mask R-CNN
* OpenCV
* NumPy

---

## Project Structure

```text
CNN-Instance-Segmentation-Using-PixelLib/
│
├── app.py
├── cycle.jpg
├── mask_rcnn_coco.h5
├── output4.jpg
└── README.md
```

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/CNN-Instance-Segmentation-Using-PixelLib.git
cd CNN-Instance-Segmentation-Using-PixelLib
```

### Install Dependencies

```bash
pip install pixellib tensorflow opencv-python numpy
```

---

## Download Pretrained Model

Download the COCO pretrained Mask R-CNN model:

* mask_rcnn_coco.h5

Place the file inside the project directory.

---

## Usage

Run the application:

```bash
python app.py
```

### Source Code

```python
from pixellib.instance import instance_segmentation

segment_image = instance_segmentation()

segment_image.load_model("mask_rcnn_coco.h5")

segment_image.segmentImage(
    "cycle.jpg",
    show_bboxes=True,
    output_image_name="output4.jpg"
)
```

---

## Input

* Image: `cycle.jpg`
* Model: `mask_rcnn_coco.h5`

---

## Output

The application generates:

* Object Labels
* Segmentation Masks
* Bounding Boxes
* Processed Output Image (`output4.jpg`)

---

## Applications

* Autonomous Vehicles
* Smart Surveillance Systems
* Traffic Monitoring
* Robotics and Automation
* Retail Analytics
* Medical Image Analysis
* Object Tracking and Recognition

---

## Future Enhancements

* Real-Time Video Segmentation
* Webcam Integration
* Custom Dataset Training
* YOLO-based Segmentation
* Flask/FastAPI Web Deployment
* Cloud-Based Inference

---

## Author

**Rahul Gorain**

Master of Computer Applications (MCA)
Dr. B.C. Roy Engineering College

### Skills

Computer Vision • Deep Learning • TensorFlow • CNN • Machine Learning • Python
