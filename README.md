# Virtual-Mouse-Using-HandRecognition

## Overview

The projects utilize Google's Mediapipe, an open-source machine learning tool, for hand tracking and recognition. These projects demonstrate various applications of hand tracking, including controlling a mouse cursor and adjusting system volume.

### Hand Tracking

This project captures and tracks hand movements in real-time, highlighting hand landmarks and providing the functionality to recognize finger gestures.

### Virtual Mouse Control

This project allows controlling the mouse cursor using hand gestures. It includes features for smooth cursor movement and left-click functionality.

### Virtual Volume Control

This project enables volume control through hand gestures, including adjusting the volume up or down and displaying the current volume level on the screen.

## Requirements

- Python 3.x
- OpenCV
- Mediapipe
- Numpy
- Autopy (for Virtual Mouse Control)
- Pycaw (for Virtual Volume Control)

Install the required packages using pip:
```sh
pip install opencv-python mediapipe numpy autopy pycaw
```

## Hand Tracking

### Description

The `handTracker` class encapsulates the hand tracking functionality, including:
- Detecting and drawing hand landmarks.
- Identifying finger positions.
- Checking which fingers are up.
- Calculating the distance between two landmarks.

### Usage

1. **Hand Tracking**:
    ```python
    import cv2
    import mediapipe as mp
    import time
    import math
    import numpy as np

    # Class definition and main function...
    ```

2. **Running the Hand Tracking**:
    ```python
    if __name__ == "__main__":
        main()
    ```

## Virtual Mouse Control

### Description

This script uses hand gestures to control the mouse cursor:
- Moving the index finger to move the cursor.
- Pinching with the index and middle fingers to perform a click.

### Usage

1. **Virtual Mouse Control**:
    ```python
    import cv2
    import numpy as np
    import handtrack as htm
    import time
    import autopy

    # Script implementation...
    ```

2. **Running the Virtual Mouse Control**:
    ```sh
    python Virtual_Mouse.py
    ```

## Virtual Volume Control

### Description

This script uses hand gestures to control the system volume:
- Moving the thumb and index finger to adjust the volume.
- Displaying the volume level on the screen.

### Usage

1. **Virtual Volume Control**:
    ```python
    import cv2
    import time
    import numpy as np
    import handtrack as htm
    import math
    from ctypes import cast, POINTER
    from comtypes import CLSCTX_ALL
    from pycaw.pycaw import AudioUtilities, IAudioEndpointVolume

    # Script implementation...
    ```

2. **Running the Virtual Volume Control**:
    ```sh
    python Virtual_Volume_Control.py
    ```

