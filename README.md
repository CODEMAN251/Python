
# Hand Gesture Controlled LED using Python, OpenCV, Mediapipe, and Firmata

This project demonstrates how to control LEDs using hand gestures detected through a webcam. The hand gestures are recognized using the Mediapipe library, and the LEDs are controlled via an Arduino Uno R3 board using the Firmata protocol. OpenCV is used to capture and process the video feed from the webcam.

## Prerequisites

- Python 3.x
- Arduino Uno R3 board
- Webcam
- Firmata library installed on the Arduino board
- Required Python libraries: mediapipe, opencv-python, pyfirmata

# Installation

1. Clone the repository:

   git clone https://github.com/CODEMAN251/Python.git


2. Install the required Python libraries:

   pip install mediapipe opencv-python pyfirmata

3. Upload Firmata to the Arduino board:

   Upload the StandardFirmata example from the Arduino IDE (File -> Examples -> Firmata -> StandardFirmata) to your Arduino board. This will enable communication between the Python script and the Arduino.

## Usage

1. Connect the LEDs to the Arduino:

   Connect the LEDs to the digital pins of the Arduino board. Make sure to connect the cathode (shorter leg) of the LED to the ground (GND) pin and the anode (longer leg) to the chosen digital pin.

2. Run the Python script:

   Navigate to the project directory and run the 'main.py` script:

   python main.py

   This will open the webcam and start detecting hand gestures. Depending on the detected hand gesture, the LEDs will be turned on, off, or controlled accordingly.

3. Interact with the LEDs:

   Follow the instructions displayed on the screen to control the LEDs using your hand gestures. Gestures such as an open hand, a closed fist, or specific finger configurations will trigger different LED states.

4. Quit the script:

   Press `q` to quit the script and close the webcam feed.

# Customization

You can customize the LED pins, gesture thresholds, and other settings by modifying the variables in the `main.py` script. Refer to the comments in the script for guidance.

#  Troubleshooting

- If you encounter issues with the Arduino not communicating correctly, ensure that you have uploaded the Firmata sketch to the board.
- Check the connections of the LEDs and verify that they are connected to the correct digital pins on the Arduino.

# Acknowledgments

This project was inspired by the possibilities of gesture-based interaction and combines the power of Mediapipe, OpenCV, and Firmata to create a unique experience.

