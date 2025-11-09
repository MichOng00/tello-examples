# Tello Drone Python Examples

This repository contains various examples of controlling and interacting with Tello drones using Python. The examples use the [DJITelloPy](https://github.com/damiafuentes/DJITelloPy) library for drone control and [MediaPipe](https://ai.google.dev/edge/mediapipe/solutions/guide) for computer vision tasks like face tracking and expression detection.

## Prerequisites

### 1. Python Version

Ensure that you are using Python 3.9. You can create a virtual environment using either `venv` or `conda`:

#### Using `venv`:

```bash
python3.9 -m venv tello_env
source tello_env/bin/activate  # For Linux/macOS
tello_env\Scripts\activate     # For Windows
```
#### Using `conda`:
```bash
conda create -n tello_env python=3.9
conda activate tello_env
```
### 2. Install Required Libraries

Once your virtual environment is set up and activated, install the necessary libraries using `pip` (or `pip3`):
```bash
pip install djitellopy mediapipe
```
This will automatically install all required dependencies, including `opencv-python` for image processing.

### 3. Configure firewall (if necessary)
If you're running into issues connecting to the Tello drone, you may need to edit your firewall rules. Make sure that the following ports are open for inbound connections:

- 8890
- 8999
- 11111

This is necessary for communication between your Python script and the drone.

