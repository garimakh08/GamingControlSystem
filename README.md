# GamingControlSystem
**GameDriveAI** is a steering wheel simulator to play games like Asphalt and other racing games with a steering wheel in hand to get experience of driving without investing a lot of money in buying a xbox controller. It is a **computer vision-based project** that transforms a webcam into a virtual steering wheel, allowing you to control left, right, and nitro functions in games. Using OpenCV, this project detects hand gestures and translates them into keystrokes for an immersive gaming experience.

## Features

- **Real-time Hand Gesture Recognition**: Detects hand positions to control left and right steering.
- **Nitro Boost Activation**: Recognizes a specific hand gesture for activating nitro boost in games.
- **Easy Setup**: Requires only a webcam and the necessary libraries to get started.

## Requirements

* Python 3.x
* OpenCV
* imutils
* numpy
* VideoStream (part of imutils)
* directkeys

## How It Works

1. **Video Capture**: The webcam captures video frames.
2. **Image Processing**: The frames are processed to detect specific color ranges.
3. **Contour Detection**: Contours are identified in the processed frames to determine hand positions.
4. **Key Press Simulation**: Based on hand positions, corresponding keystrokes (left, right, nitro) are simulated.

## Usage

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/GameDriveAI.git
    cd GameDriveAI
    ```

2. Install the required libraries:
    ```sh
    pip install numpy opencv-python imutils
    ```

3. Run the script:
    ```sh
    python gamedrive_ai.py
    ```

4. Use the following hand gestures to control the game:
    - **Move Left**: Move your hand to the left side of the screen.
    - **Move Right**: Move your hand to the right side of the screen.
    - **Activate Nitro**: Move your hand to the bottom center of the screen.

Press 'q' to quit the application.
