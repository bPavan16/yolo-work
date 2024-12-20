
# People Counter

This project is a People Counter using the YOLO (You Only Look Once) object detection algorithm. The system counts the number of people in a given video feed or image.

## Features

- Real-time people counting
- High accuracy with YOLO algorithm
- Easy to use and integrate

## Requirements

- Python 3.x
- OpenCV
- NumPy
- YOLOv8 weights and configuration files

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/People-Counter.git
    ```
2. Navigate to the project directory:
    ```bash
    cd People-Counter
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Download the YOLOv8 weights and configuration files from the [official YOLO website](https://pjreddie.com/darknet/yolo/).
2. Place the downloaded files in the `yolo` directory.
3. Run the people counter script:
    ```bash
    python people_counter.py --input path_to_video_or_image --output path_to_output
    ```

## Example

```bash
python people_counter.py --input sample_video.mp4 --output output_video.avi
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

