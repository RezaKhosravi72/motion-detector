# Motion Detection using OpenCV and Python

This Python project utilizes the OpenCV library to detect motion in live video from the default camera. It provides real-time visualization of detected motion on the screen and records the start and end times of motion events in a CSV file.

## How it works

- The program captures video from a webcam
- Computes frame differences between current and previous frames
- Thresholds the differences to get a binary image with motion areas
- Performs morphological dilation to combine fragmented blobs  
- Finds contours in thresholded frame to detect motion regions
- Tracks frame-to-frame changes in motion status
- Logs timestamps of detected motions to a CSV file

## Requirements

- Python 3
- OpenCV 
- Pandas

## Usage

1. Clone this repo
2. Install requirements `pip install -r requirements.txt`
3. Run `python motion_detector.py`
4. Press 'q' to exit and save timestamps 

This will open the camera stream and display output frames. Detected motion regions will be outlined.

## Possible Improvements

- Track detected blobs between frames
- Filter spurious detections using size/duration thresholds
- Classify motion type (person, vehicle etc.) using Deep Learning
- Run on video file instead of webcam
- Add GUI controls
- Deploy on edge device for real-time monitoring

## Applications

- Security & surveillance 
- Traffic monitoring
- Industrial quality control  
- Animal behavior studies
- Motion-based control interfaces

