# Unified Object Detection Projects

This repository hosts multiple projects leveraging state-of-the-art YOLO (You Only Look Once) models for real-time object detection across various domains. Each project highlights specific use cases, including dental anatomy detection, people counting, and lane change detection.

## Projects Overview

### 1. Dental Anatomy Detection System
This project uses YOLOv11 to detect and classify different types of teeth in dental images, labeling them with their anatomical names.

#### Features
- Detects and classifies molars, premolars, canines, and incisors.
- Provides high-accuracy detection and labeling.

#### Prerequisites
- Python 3.x
- OpenCV
- NumPy
- Pillow
- YOLOv11 pre-trained weights

#### Usage
1. Prepare dental images.
2. Download YOLOv11 weights and configuration.
3. Run the detection script to output labeled images.

---

### 2. People Counter
This project counts the number of people in a given video feed or image using YOLO.

#### Features
- Real-time people counting.
- High accuracy with YOLO.

#### Requirements
- Python 3.x
- OpenCV
- NumPy
- YOLO weights and configuration files.

#### Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/People-Counter.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Download YOLO weights and run the script:
   ```bash
   python people_counter.py --input path_to_video_or_image --output path_to_output
   ```

---

### 3. Lane Change Detection
This project uses YOLOv8 to detect lane changes in real-time from video feeds.

#### Features
- Enhanced lane change detection accuracy using YOLOv8.
- Real-time object detection.

#### Requirements
- Python 3.x
- OpenCV
- NumPy
- YOLOv8 pre-trained weights
- Ultralytics library

#### Usage
1. Install YOLOv8:
   ```bash
   pip install ultralytics
   ```
2. Load YOLOv8 and process the video:
   ```python
   from ultralytics import YOLO

   model = YOLO('yolov8.pt')
   results = model.detect('video.mp4')
   ```
3. Run the Jupyter notebook to detect and display lane changes.

---

## Installation

For all projects:
1. Clone the repository.
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the appropriate YOLO weights and configuration files.

## License
This repository is open-source and available under the MIT License.

## Acknowledgments
- OpenCV for image processing.
- YOLOv8 and YOLOv11 for state-of-the-art object detection.
- NumPy for numerical operations.
- Pillow for image annotation.
- Ultralytics for YOLOv8 support.

