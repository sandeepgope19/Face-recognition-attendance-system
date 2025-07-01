# Face Recognition Attendance System

This project implements a **Face Recognition Attendance System** using Python, OpenCV, and Keras. The system leverages a pre-trained convolutional neural network model to recognize faces and record attendance automatically in real time.

## Features
- **Real-Time Face Detection**: Uses Haar Cascade Classifier to detect faces from live video feeds.
- **Face Recognition**: Identifies faces using a pre-trained CNN model and maps them to predefined labels.
- **Automated Attendance**: Automatically logs attendance upon successful recognition of faces.
- **Preprocessing**: Implements image preprocessing techniques such as grayscale conversion, histogram equalization, and resizing for better accuracy.

## Requirements
- Python 3.8 or later
- OpenCV
- Keras
- NumPy
- urllib
- os
- pickle

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/sandeepgope19/Face-recognition-attendance-system
   cd face-recognition-attendance-system
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Add the required files:
   - Haar Cascade XML file (`haarcascade_frontalface_default.xml`) for face detection.
   - Trained model (`fianl_model.h5`) for face recognition.
   - Data files (`images` and `labels`) in the appropriate directory.
   - images file (`image.jpg`) for testing.

## How It Works
1. **Data Preprocessing**: Images are resized, converted to grayscale, and normalized before being fed into the model.
2. **Face Detection**: The system detects faces in real-time from the live feed using Haar Cascade Classifier.
3. **Prediction**: The pre-trained model identifies the detected face and assigns a label.
4. **Attendance Logging**: Recognized faces are recorded, and attendance is updated automatically.

## Usage
1. Start the script:
   ```bash
   python recognize.py
   ```
2. Ensure the video feed is active and faces are in clear view for detection and recognition.
3. Press `q` to quit the application.

## File Structure
- `consolidated_data.py`: Script to preprocess and save image data and labels.
- `recognize.py`: Main script for face recognition and attendance logging.
- `haarcascade_frontalface_default.xml`: Haar Cascade file for face detection.
- `fianl_model.h5`: Pre-trained model for face recognition.

## Future Enhancements
- Add a GUI for easier user interaction.
- Enable database integration for attendance records.
- Improve model accuracy with a larger training dataset.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- OpenCV for face detection tools.
- Keras for enabling model training and deployment.
- The open-source community for providing resources and support.

## Author
[Sandeep Gopw]
[sandeepgope19@gmail.com]
