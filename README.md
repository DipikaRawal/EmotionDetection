# Real-Time Emotion Recognition using face-api.js

## Introduction
This project implements real-time facial emotion recognition in the browser using [face-api.js](https://github.com/justadudewhohacks/face-api.js), a JavaScript API built on top of TensorFlow.js. It enables face detection, face recognition, and expression analysis directly from webcam input.

## Features
- **Real-time Face Detection**: Uses `face-api.js` models to detect faces in a live video feed.
- **Emotion Recognition**: Identifies facial expressions such as happy, sad, angry, surprised, etc.
- **Web-Based**: Runs entirely in the browser without requiring external servers.

## Installation
### 1. Clone the Repository
```bash
git clone https://github.com/DipikaRawal/EmotionDetection
cd face-api-emotion-recognition
```

### 2. Install Dependencies
If you are using npm, install dependencies with:
```bash
npm install
```
Alternatively, you can use a CDN to include `face-api.js`:
```html
<script defer src="https://cdn.jsdelivr.net/npm/@vladmandic/face-api@latest/dist/face-api.min.js"></script>
```

## Usage
### 1. Start a Local Server
For local development, you can start a simple HTTP server:
```bash
npx serve .
```
Then, open `http://localhost:3000` in your browser.

### 2. Turn on the Webcam
The application will request permission to access your webcam. Allow it to proceed.

### 3. Load Models
The required models will be loaded dynamically when the page initializes.

### 4. Detect Faces & Recognize Emotions
Once the models are loaded, the application will start detecting faces and classifying emotions in real-time.

## Models Used
- **Face Detection**:
  - `SSD Mobilenet V1`: High accuracy but slower.
  - `Tiny Face Detector`: Faster and optimized for mobile.
- **Face Landmark Detection**: Identifies 68 facial landmarks.
- **Face Recognition**: Computes a 128-dimension feature vector.
- **Face Expression Recognition**: Classifies emotions with a lightweight model.

## Technologies Used
- **JavaScript**
- **face-api.js** (built on TensorFlow.js)
- **HTML5 & CSS3**

## Known Issues
- Accuracy may decrease for small or partially occluded faces.
- Wearing glasses can impact emotion detection.

## Future Improvements
- Improve UI for better visualization of detected emotions.
- Implement multi-face tracking.
- Add support for additional facial attributes (e.g., age, gender estimation).


---
Feel free to contribute or report issues! 🚀

