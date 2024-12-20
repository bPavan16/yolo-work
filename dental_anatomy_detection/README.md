# Dental Anatomy Detection System

This project implements a dental anatomy detection system using YOLOv11 (You Only Look Once) object detection model. The system identifies and classifies various types of teeth in dental images and labels them appropriately.

## Features
- Detects and classifies different types of teeth (e.g., molars, premolars, canines, incisors) in dental images.
- Labels detected teeth with their anatomical names.
- Supports high-accuracy detection using the latest YOLOv11 model.

## Prerequisites

To run the code, ensure you have the following dependencies installed:

- Python 3.x
- OpenCV
- NumPy
- Pillow
- YOLOv11 pre-trained model (download the weights from the official YOLO repository or a relevant source).

Install the required Python libraries using the following command:
```bash
pip install opencv-python numpy pillow
```

## Usage

1. **Prepare the Input Data**:
   - Ensure you have a set of dental images ready for processing. Place these images in a directory accessible to the script.

2. **Download YOLOv11 Weights**:
   - Download the YOLOv11 pre-trained weights and configuration files for dental anatomy detection.

3. **Run the Detection Script**:
   - Execute the script in a Python environment. The script will process each input image and display the results with labeled teeth.

4. **Inspect Results**:
   - The system outputs annotated images with bounding boxes and labels for each detected tooth.

## Code Walkthrough

1. **Model Initialization**:
   - The YOLOv11 model is loaded using the appropriate configuration and weights files:
     ```python
     model = YOLOv11('path_to_weights')
     ```

2. **Image Preprocessing**:
   - Input images are resized and normalized to meet the requirements of YOLOv11.

3. **Object Detection**:
   - YOLOv11 processes each image to detect teeth and classify them into categories such as molars, premolars, canines, and incisors.

4. **Annotation**:
   - The system draws bounding boxes around detected teeth and labels them with their anatomical names.

5. **Display Results**:
   - Annotated images are displayed or saved to an output directory for further review.

## Customization

- **Model Training**: Retrain YOLOv11 with a custom dataset if needed for higher accuracy in specific dental images.
- **Class Labels**: Update the class labels to include additional categories or specific annotations (e.g., wisdom teeth).
- **Output Format**: Modify the script to save the results in a preferred format 
## Example Output
When running the script, the system outputs annotated images with bounding boxes and labels for each detected tooth:

## Limitations
- The system relies on the accuracy of the YOLOv11 model. Ensure the model is trained on a comprehensive dental dataset.
- Image quality and resolution may affect detection performance.

## License
This project is open-source and available under the MIT License.

## Acknowledgments
- OpenCV for image processing
- YOLOv11 for object detection
- NumPy for numerical operations
- Pillow for image annotation and display

