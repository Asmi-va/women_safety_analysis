
---

# Women Safety Analytics

## Overview

This project is designed to enhance women's safety through real-time video analysis. It uses machine learning and computer vision techniques to detect faces, classify gender, identify gestures, and generate alerts based on suspicious behavior. Key functionalities include:
- Face detection
- Gender classification
- Gesture recognition
- Real-time alert system for lone women and suspicious gestures

## Features
- **Face Detection:** Uses OpenCV's pre-trained model for detecting faces in video frames.
- **Gender Classification:** Classifies detected faces into male or female using a deep learning model.
- **Gesture Recognition:** Placeholder for gesture detection model (needs implementation).
- **Alert System:** Sends email alerts and displays on-screen notifications for detected anomalies, lone women, or suspicious gestures.

## Setup

### Prerequisites
- Python 3.x
- OpenCV
- TensorFlow (for gesture recognition, if applicable)
- NumPy
- smtplib (for sending email alerts)

### Installation

1. **Clone the Repository**
   ```bash
   git clone(https://github.com/Asmi-va/women_safety_analysis/new/main?readme=1)
   cd repository
   ```

2. **Install Dependencies**
   ```bash
   pip install opencv-python numpy
   ```

3. **Download Pre-trained Models**
   - Download the following models and place them in the project directory:
     - [Face detection model](https://github.com/opencv/opencv/tree/master/samples/dnn)
     - [Age detection model](https://github.com/opencv/opencv/tree/master/samples/dnn)
     - [Gender detection model](https://github.com/opencv/opencv/tree/master/samples/dnn)
     - [Gesture recognition model]

4. **Configure Email Alerts**
   - Update the `EMAIL_HOST`, `EMAIL_PORT`, `EMAIL_HOST_USER`, `EMAIL_HOST_PASSWORD`, and `ALERT_RECEIVER` variables in the code with your SMTP server details and email addresses.

### Running the Application

1. **Start the Script**
   ```bash
   python women_safety_analysis.py
   ```

2. **Terminate the Script**
   - Press `q` in the OpenCV window to stop the video capture.

## Project Structure

```
women_safety_analysis/
├── women_safety_analysis.py
├── opencv_face_detector.pbtxt
├── opencv_face_detector_uint8.pb
├── age_deploy.prototxt
├── age_net.caffemodel
├── gender_deploy.prototxt
├── gender_net.caffemodel
├── gesture_recognition_model.h5
├── women_safety.log
└── README.md
```

## Known Issues
- Gesture recognition model is currently a placeholder and needs to be implemented.
- Ensure all models are correctly downloaded and paths are updated in the script.

## Contributing

Feel free to contribute to this project by opening issues or submitting pull requests. For detailed contribution guidelines, please refer to [CONTRIBUTING.md](CONTRIBUTING.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

