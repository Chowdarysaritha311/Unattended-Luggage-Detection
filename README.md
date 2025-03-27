Unattended Luggage Detection

Overview

This project is an AI-powered surveillance system that detects unattended luggage and determines how long a specific luggage ID remains stationary. It helps improve security in public places by alerting authorities when a piece of luggage is left unattended for too long.

Features

✅ Real-Time Luggage Detection – Uses YOLO for fast and accurate object detection.
✅ Multi-Object Tracking – Assigns unique IDs to each luggage item and tracks them using Deep SORT.
✅ Stationary Time Monitoring – Tracks how long luggage remains in the same location.
✅ Automated Alerts – Notifies security personnel via alerts when luggage is left unattended.
✅ Lightweight & Optimized – Uses efficient models for real-time processing.
✅ Works in Various Conditions – Adaptable to different lighting and environmental conditions.

How It Works

1. Detect Luggage – The system detects luggage in a live video stream using YOLO.


2. Assign IDs & Track Motion – Each luggage is assigned an ID and tracked using Deep SORT.


3. Monitor Stationary Time – The system checks if luggage remains in the same spot beyond a threshold.


4. Trigger Alerts – If the luggage is unattended for too long, an alert is sent.



Technologies Used

Python, OpenCV – For image processing and real-time video analysis.

YOLOv8 / YOLOv5 – Object detection for identifying luggage.

Deep SORT – Multi-object tracking for assigning unique IDs.

NumPy, Pandas – Data handling and time monitoring.

Flask / FastAPI – Web dashboard for monitoring alerts (Optional).


Installation

1. Clone the Repository

git clone https://github.com/your-username/Unattended-Luggage-Detection.git
cd Unattended-Luggage-Detection

2. Install Dependencies

pip install -r requirements.txt

3. Download Pre-Trained Model (YOLOv8 or YOLOv5)

# Example for YOLOv8
wget https://github.com/ultralytics/yolov8/releases/download/v8.0/yolov8n.pt

4. Run the System

python detect_luggage.py --source video.mp4

Usage

Live Camera Feed: Run the script with --source 0 for webcam input.

Custom Video Files: Specify a video file path as --source video.mp4.

Alert System: Customize alert threshold (e.g., send an alert if luggage is unattended for 5 minutes).


Real-World Applications

Airports & Railway Stations – Prevent unattended baggage threats.

Shopping Malls & Public Places – Reduce theft and safety risks.

Smart City Surveillance – Enhance real-time security monitoring.


Pros & Cons

✅ Pros

✔️ Enhances security and public safety.
✔️ Works in real-time with minimal delay.
✔️ Adaptable to different environments and conditions.
✔️ Can be integrated with existing surveillance systems.

❌ Cons

✖️ Requires computational power for real-time processing.
✖️ May have detection limitations in extremely crowded areas.
✖️ False alarms can occur due to movement misinterpretation.


---

Contribute

Feel free to fork this repository and contribute by improving detection accuracy, adding new alert mechanisms, or optimizing tracking algorithms.

License

This project is open-source under the MIT License.
