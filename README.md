# Video Processing with Object Tracking and Segmentation

This project processes a video file to perform object tracking using the dlib correlation tracker and YOLO-based detection. Additionally, the SAM (Segment Anything Model) is used to generate segmentation masks, applying a grayscale effect to areas outside the segmented object.

## Features
- **YOLO Detection**: Periodically resets the tracker with YOLO detections for improved accuracy.
- **Dlib Tracker**: Tracks objects across frames using correlation tracking.
- **Segmentation with SAM**: Applies segmentation masks for focused processing.
- **Grayscale Effect**: Highlights the tracked object by converting the rest of the frame to grayscale.
- **Output Video**: Saves the processed video in a specified format.

## Prerequisites
- Python 3.7 or later
- Required libraries:
  - `torch`
  - `dlib`
  - `cv2` (OpenCV)
  - `numpy`

Install the required libraries using:
```bash
pip install -r requirements.txt
