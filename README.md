# Accurate Head Extraction

This repository contains a simple web-based application that uses the `face-api.js` library to detect faces in uploaded images and extract heads with precise bounding box calculations. The extracted heads are resized and displayed as smaller images, suitable for further processing.

## Features

- Detects faces in uploaded images using the `TinyFaceDetector` model from `face-api.js`.
- Extracts head regions with accurate bounding boxes based on facial landmarks.
- Resizes and compresses extracted heads to fit within 99KB, ensuring optimized image size.
- Displays the processed images with their respective file sizes.

## Demo

### How It Works:
1. **Upload an Image**: Users can upload an image file.
2. **Face Detection**: The app detects faces and landmarks, including eyebrows and jawlines.
3. **Head Extraction**: It calculates bounding boxes that closely fit the head region and extracts it from the original image.
4. **Image Resizing**: The extracted heads are resized to meet a maximum size constraint (99KB) while maintaining quality.
5. **Output Display**: The processed images are shown along with their size in kilobytes.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/accurate-head-extraction.git
   ```

2. Serve the `index.html` file locally or deploy it on any web server.

## Usage

1. Open the `index.html` file in a modern browser (preferably Chrome or Firefox).
2. Click the "Choose File" button to upload an image.
3. The app will process the image and extract the heads, which will be displayed below the upload area.

## Libraries Used

- **[face-api.js](https://github.com/justadudewhohacks/face-api.js)**: A JavaScript library that uses neural networks to detect faces and facial landmarks.
- **HTML5 Canvas**: Used to draw and manipulate images.

## Customization

- **Face Detection Parameters**: The detection model uses the `TinyFaceDetectorOptions`. You can adjust the `inputSize` and `scoreThreshold` to improve performance for different image types.
- **Bounding Box Adjustment**: The script calculates custom bounding boxes based on landmarks. You can tweak these to capture different parts of the face or head.
  
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to contribute or report issues!
