
# Digit Recognition from Screen Capture

This program captures a portion of the screen, processes the image, and uses a pre-trained model to recognize handwritten digits.

## Features
- Real-time screen capture of a specified region
- Image preprocessing (grayscale conversion, Gaussian blur, thresholding)
- Digit prediction using a pre-trained machine learning model
- Display of prediction results on the captured image

## Requirements
- Python 3.x
- Required packages:




joblib
opencv-python (cv2)
numpy
pyscreenshot

text

## Installation
1. Clone this repository or download the project files
2. Install the required packages:

pip install joblib opencv-python numpy pyscreenshot
Place your trained model file (digit_recognizer) in the model/ directory

Create an img/ directory for temporary image storage

Usage
Run the program:

bash
python digit_recognizer.py
The program will:

Capture the screen region defined by the bbox coordinates (60,170,400,500)

Process the image and make a prediction

Display the result in a window

Press Enter to exit the program

File Structure
text
project/
│── digit_recognizer.py    # Main program file
│── model/
│   └── digit_recognizer   # Pre-trained model file
└── img/                   # Directory for captured images
    └── img.png            # Temporary image file
Configuration
You can modify these parameters in the code:

Screen capture region: Change the bbox coordinates in ImageGrab.grab()

Image processing: Adjust threshold values, blur parameters

Display: Change the prediction display text properties

Notes
The program currently captures a fixed region of the screen

The model expects 28x28 pixel grayscale images

The threshold value (100) may need adjustment based on your screen/background

License
[Specify your license here, e.g., MIT, GPL, etc.]

text

This README includes:
1. Project description
2. Features list
3. Installation instructions
4. Usage guide
5. File structure explanation
6. Configuration options
7. Important notes
8. License information

You can customize it further by:
- Adding screenshots of the program in action
- Including information about how the model was trained
- Adding contribution guidelines
- Providing contact information for support
