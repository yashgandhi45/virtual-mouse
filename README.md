# Virtual Mouse using Hand Gestures

This project demonstrates a **virtual mouse control** system using hand gestures. It allows you to control the mouse pointer and perform clicks using the position of your hand detected by a webcam. The project uses **OpenCV**, **MediaPipe**, and **PyAutoGUI** to achieve this functionality.

## Features
- **Mouse Movement**: Move the mouse pointer using your hand's index finger.
- **Mouse Click**: Perform a left-click using the index and middle fingers together.
- **Smooth Mouse Movement**: The pointer movement is smoothed for better usability.
- **Real-time Finger Detection**: Detects finger positions in real-time and translates them to mouse actions.

## Requirements

Make sure you have Python 3.x installed. To install the required libraries, run the following command:

```bash
pip install opencv-python mediapipe pyautogui numpy
```

## Setup & Usage

1. **Clone the Repository:**

   Clone this repository to your local machine using Git:

   ```bash
   git clone https://github.com/yashgandhi45/virtualmouse.git
   ```

2. **Run the Code:**

   After installing the required libraries, you can run the script. Simply execute the following command:

   ```bash
   python virtualmouse.py
   ```

3. **How It Works:**

   - **Hand Detection**: The system uses MediaPipe to detect and track hand landmarks in real-time.
   - **Finger Detection**: It detects whether your index or middle finger is raised to perform specific actions.
   - **Mouse Control**: The mouse cursor will move based on the position of your hand, and clicking occurs when the index and middle fingers are close enough.

4. **Control Instructions**:
   - **Move the Mouse**: Raise only the **index finger**.
   - **Click the Mouse**: Raise both the **index and middle fingers** close together.

## Code Explanation

The project utilizes two main components:
- **HandDetector Class**: A class to handle the detection of hand landmarks and fingers, as well as the mouse control logic.
- **Main Program**: Captures webcam input and processes the hand gestures to move the mouse and perform clicks.
