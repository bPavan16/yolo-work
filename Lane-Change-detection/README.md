## Using YOLOv8 for Lane Change Detection

This project leverages YOLOv8 for object detection to enhance lane change detection accuracy. YOLOv8 is a state-of-the-art object detection model that provides real-time performance and high accuracy.

### Installation

To use YOLOv8, you need to install additional dependencies:

```sh
pip install ultralytics
```

### Usage

1. Ensure your video file is in the project directory and named `video.mp4`.

2. Modify the Jupyter notebook to include YOLOv8 for object detection:

   ```python
   from ultralytics import YOLO

   # Load the YOLOv8 model
   model = YOLO('yolov8.pt')

   # Process the video and detect objects
   results = model.detect('video.mp4')
   ```

3. Run the Jupyter notebook:

   ```sh
   jupyter notebook notebook.ipynb
   ```

4. The notebook will process the video, detect objects using YOLOv8, and display frames with detected lane changes.

By integrating YOLOv8, the project can more accurately detect vehicles and their lane changes, improving the overall performance of the lane change detection system.
