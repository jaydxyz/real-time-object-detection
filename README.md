# Real-Time Object Detection with OpenCV and YOLO

This project demonstrates real-time object detection using Python, OpenCV, and the YOLO (You Only Look Once) object detection model. The application can identify and locate various objects in video streams from a webcam or a provided video file in real-time.

## Features

- Real-time object detection using webcam footage or any video file provided by the user
- Integration with the pre-trained YOLO model for accurate object detection
- Bounding box visualization around detected objects with labels showing the classification
- Display of performance metrics such as frame rate and detection accuracy in real-time

## Prerequisites

Before running the script, ensure that you have the following dependencies installed:

- Python 3.x
- OpenCV: Install using `pip install opencv-python`
- NumPy: Install using `pip install numpy`

You will also need the YOLO model files:

- `yolov4.weights`: Download the pre-trained YOLO weights file from the official YOLO website or a reliable source.
- `yolov4.cfg`: Download the YOLO configuration file that defines the model architecture.
- `coco.names`: Download the COCO dataset class names file, which contains the names of the objects that YOLO can detect.

Place these files in the same directory as the Python script.

## Usage

1. Clone the repository or download the Python script and the required YOLO model files.

2. Open a terminal or command prompt and navigate to the project directory.

3. Run the script using the following command:
   ```
   python object_detection.py
   ```

4. The script will open a window displaying the real-time video stream with object detection overlay.

5. To use a webcam, ensure that a webcam is connected to your computer. The script will automatically use the default webcam (index 0).

6. To use a video file instead of a webcam, provide the path to the video file in the `cv2.VideoCapture()` function call in the script.

7. Press 'q' to quit the application.

## Customization

- To use a different YOLO model version (e.g., YOLOv3), download the corresponding model files and update the file paths in the script accordingly.

- Adjust the confidence threshold and non-maximum suppression threshold in the script to fine-tune the object detection performance.

## Acknowledgements

- The YOLO object detection model is developed by Joseph Redmon et al. For more information, refer to the [YOLO website](https://pjreddie.com/darknet/yolo/).

- The OpenCV library is used for video capture and image processing. Visit the [OpenCV website](https://opencv.org/) for more details.

## License

This project is licensed under the [MIT License](LICENSE).
