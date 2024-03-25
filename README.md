# Crowd Detection in Video and Live Webcam Feeds

Introduction:
This project aims to detect and track people in both video files and live webcam feeds using computer vision techniques. The detection and tracking are performed using the YOLO (You Only Look Once) object detection algorithm, and the DeepSORT (Deep Simple Online and Realtime Tracking) algorithm for tracking.

Features:

Live Webcam Feed: Users can access a live webcam feed where the system detects and tracks people in real-time.
Video Processing: Users can upload a video file, and the system will process it to detect and track people throughout the video duration.
Object Detection: The system employs YOLOv5 for object detection, specifically focusing on detecting people from the video frames or webcam feed.
Tracking: After detection, DeepSORT is used to track the detected people across frames, maintaining their identities throughout the video or live feed.
Visualization: Detected people are highlighted with bounding boxes and labels, making it easy for users to visualize and understand the tracking process.
Counting: The system counts the number of people detected in the frame or feed, providing insights into crowd density.
Technologies Used:

Flask: The web application framework used for building the user interface and handling HTTP requests.
OpenCV: Used for capturing video from the webcam, processing video files, and performing real-time object detection and tracking.
PyTorch: Utilized for loading and running the YOLOv5 object detection model.
DeepSORT: A deep learning-based object tracking algorithm used for associating detections with existing tracks and creating new tracks when necessary.
Ultralytics YOLO: A PyTorch-based implementation of YOLOv5 for object detection.
HTML/CSS: For designing the user interface and styling web pages.
Usage:

Accessing the Web Application: Users can access the web application by running the Flask server locally or deploying it to a server accessible over the network.
Live Webcam Feed: Upon accessing the web application, users can navigate to the live webcam feed page to view real-time crowd detection and tracking.
Video Processing: Users can upload video files through the web interface, and the system will process them to detect and track people. The processed video can then be viewed or downloaded.
How to Run:

Clone the repository to your local machine.
Install the required dependencies listed in the requirements.txt file.
Run the Flask application by executing the Python script app.py.
Access the web application through a web browser using the provided URL (typically http://localhost:5000).
Navigate through the different pages to explore the live webcam feed and video processing features.
Contributions:
Contributions to this project are welcome. You can contribute by:

Adding new features or enhancements to improve the functionality or user experience.
Fixing bugs or issues reported by users.
Optimizing the code for better performance or resource utilization.
License:
This project is licensed under the MIT License. See the LICENSE file for more details.

Acknowledgments:

The YOLOv5 implementation by Ultralytics provided a robust solution for object detection.
The DeepSORT algorithm implementation was instrumental in enabling object tracking across frames.
