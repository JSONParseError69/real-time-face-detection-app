# Face Recognition with Age and Gender Detection

This project demonstrates real-time face detection, age estimation, and gender recognition using the [face-api.js](https://github.com/justadudewhohacks/face-api.js) library. The application accesses the user's webcam and displays facial landmarks, expressions, as well as predicted age and gender directly on the video feed.

## Features

- Real-time face detection using the Tiny Face Detector
- Face landmarks detection
- Facial expression recognition
- Age estimation
- Gender recognition

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/JSONParseError69/real-time-face-detection-app
   cd real-time-face-detection-app
   ```

2. Install the necessary dependencies:

- This project relies on face-api.js and basic HTML/CSS/JS files, so no additional dependencies are needed.

Download the models:

- Download the face-api.js models from here and place them in a /models directory in the root of your project.

## Usage

1. Open the index.html file in your browser. You can do this by simply dragging and dropping the file into a browser window or by serving the file with a local server.

2. Allow camera access when prompted.

3. You should see your webcam feed with real-time age, gender, and expression detection.

## Code Overview

- index.html: The main HTML file that sets up the video element and loads the necessary scripts.
- script.js: Contains the core logic for initializing the video stream and running the face-api.js detection.
- style.css: Basic styling for the webpage.

## Key Code Sections

```javascript
const detections = await faceapi
  .detectAllFaces(video, new faceapi.TinyFaceDetectorOptions())
  .withFaceLandmarks()
  .withFaceExpressions()
  .withAgeAndGender();
```

This snippet captures all face detections, landmarks, expressions, and age/gender information in real-time.

## Contributing

Feel free to fork the repository and submit pull requests. Contributions are welcome!

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- face-api.js - A powerful library for face detection and recognition.
- Inspiration and support from all the amazing developers who contribute to open source.
