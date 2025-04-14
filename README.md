# Object & Person Detection with Navigation & Text Recognition

This web-based project integrates **Object Detection**, **Navigation Assistance**, and **Text Recognition** to provide an interactive and accessible experience for users. By leveraging the power of **TensorFlow.js**, **Tesseract.js**, and the **Web Speech API**, the application can detect objects in real-time through a live camera feed, help users navigate to destinations using voice commands, and read text from images using optical character recognition (OCR).

## Features
### 1. **Object Detection**
- **Real-time Object Recognition**: Uses TensorFlow.js with the COCO-SSD model to detect objects in the live video feed.
- **Bounding Box & Labeling**: Objects detected are highlighted with bounding boxes and labels on the video stream.
- **Speech Feedback**: Identified objects are announced aloud, allowing visually impaired users to interact seamlessly.

### 2. **Navigation Assistance**
- **Voice Commands for Navigation**: Users can speak destinations and choose travel modes (driving, walking, etc.), and the system will open Google Maps for directions.
- **Static Map Display**: A static map preview is shown for users to get a quick overview of their route.
- **Speech Synthesis**: Directions are announced through speech, providing step-by-step navigation.

### 3. **Text Recognition (OCR)**
- **Live Text Extraction**: Uses Tesseract.js to recognize and extract text from the camera feed.
- **Speech Output**: Extracted text is spoken out loud, making it useful for reading signs, documents, and more.
- **Error Handling**: If no text is detected, users are prompted to try again.

## Setup Instructions
1. **Clone the repository**:
    ```bash
    git clone https://github.com/MahikaTrivedi/ViSiON-46.git
    ```

2. **Open the `index.html` file** in any modern browser that supports:
   - Web Speech API
   - TensorFlow.js
   - Tesseract.js

3. **Ensure Internet Access**:
   - The project loads models and external resources, so an active internet connection is required for object detection and OCR functionalities.

## Technologies Used
- **TensorFlow.js**: Used for real-time object detection with the **COCO-SSD** model.
- **Tesseract.js**: Optical character recognition for live text extraction from video.
- **Web Speech API**: Allows speech synthesis and speech recognition for voice commands and feedback.
- **HTML5 & CSS**: For creating the UI and styling of the web page.

## How It Works
- **Camera Access**: The application uses the device's camera to stream video in real time.
- **Object Detection**: The video is passed through the COCO-SSD model to detect objects and their bounding boxes.
- **OCR**: The captured video frames are processed using Tesseract.js to extract any readable text.
- **Speech Interaction**: Users can input commands using voice recognition, and the system will respond by speaking the results aloud or opening Google Maps for navigation.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Note
- You will need a Google Maps API key for full navigation functionality.
- Make sure to replace `YOUR_GOOGLE_MAPS_API_KEY` in the code with your actual API key.

---

For more detailed instructions, refer to the source code or visit the official documentation for TensorFlow.js and Tesseract.js.
