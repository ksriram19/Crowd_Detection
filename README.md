
# Crowd Detection in Video and Live Webcam Feeds

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
[![YOLOv5](https://img.shields.io/badge/YOLOv5-v5.0-blue)](https://github.com/ultralytics/yolov5)



## Overview

This project utilizes **YOLOv5** for real-time object detection and **DeepSORT** for robust tracking to detect and track people in both video files and live webcam feeds. It features the following capabilities:

- **Real-time Crowd Detection:** Detect and track people through live webcam feeds.
- **Video Processing:** Upload and process video files to detect and track people throughout the video duration.
- **Visualizations:** Bounding boxes and labels highlight detected people in each frame.
- **Crowd Density Insights:** Count the number of people detected in real-time.

## Features

- **Accurate Detection:** YOLOv5 ensures precise identification of people within video frames.
- **Robust Tracking:** DeepSORT associates detections with existing tracks and maintains identities across frames.
- **Flexible Input Sources:** Supports both live webcam feeds and video file uploads.
- **Real-Time Processing:** Detect and track crowds as they appear in the video feed.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/crowd-detection.git
   cd crowd-detection
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

3. Download the YOLOv5 model weights:
    ```bash
   wget https://github.com/ultralytics/yolov5/releases/download/v5.0/yolov5s.pt
    ```

## Usage

### Live Webcam Feed

Run the following command to start crowd detection on a live webcam feed:
 ```bash
python detect.py --source 0  # 0 is the default webcam device ID
 ```
### Video File Processing

To process a video file for crowd detection, use:
 ```bash
python detect.py --source path/to/video.mp4
 ```
### Output Visualization

The system will provide real-time visualizations with bounding boxes and labels for each detected person, along with crowd density insights.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue for any improvements or suggestions.

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
