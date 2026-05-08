# Face Blurring System

## Overview
A Computer Vision project built using Python, OpenCV, and MediaPipe for detecting and blurring faces in:

- Images
- Videos
- Live Webcam Stream

The project automatically detects faces and applies a blur filter to preserve privacy and hide identities.

---

## Features
- Face detection using MediaPipe
- Face blurring on images
- Face blurring on videos
- Real-time webcam face blurring
- Automatic output saving
- Lightweight and fast processing

---

## Technologies Used
- Python
- OpenCV
- MediaPipe

---

## Project Structure

```bash
face-blurring/
│
├── main.py
├── blaze_face_short_range.tflite
├── outputvid.mp4
├── imout.jpg
└── README.md
```

---

## Installation

### Clone the repository

```bash
git clone <your-repo-url>
cd face-blurring
```

### Install dependencies

```bash
pip install opencv-python mediapipe
```

---

## How It Works

### 1. Image Face Blurring
- Reads an input image
- Detects faces using MediaPipe
- Applies blur on detected faces
- Saves the processed image

### 2. Video Face Blurring
- Reads video frames
- Detects faces frame by frame
- Applies blur effect
- Saves processed video as `outputvid.mp4`

### 3. Real-Time Webcam Blurring
- Captures webcam frames
- Detects faces live
- Applies blur instantly
- Displays live blurred stream

---

## Run the Project

```bash
python main.py
```

Press `q` to quit the webcam stream.

---

## Output Examples

### Image Output
- `imout.jpg`

### Video Output
- `outputvid.mp4`

---

## Notes
- Make sure the model file `blaze_face_short_range.tflite` exists in the project directory.
- Good lighting improves face detection accuracy.
- Blur intensity can be adjusted by changing:

```python
(75,75)
```

or

```python
(50,50)
```

---

## Future Improvements
- Mosaic blur support
- Face tracking
- GPU acceleration
- Emotion detection
- Face anonymization for CCTV systems

---

## Author
Developed by Mohaned Gaming