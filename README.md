# ML Face Detection

This project involves creating a face detection system using TensorFlow, OpenCV, and Albumentations.

## Installation

Before running any cells, ensure you have the necessary libraries installed. You can install them using the following command:

```sh
pip install labelme tensorflow opencv-python matplotlib albumentations
```

# Project Structure

Ensure the following directories are in the same location as your Jupyter Notebook file:
- `data`
- `aug_data`

## Instructions

### Capture Images
- This step will open your camera, capture pictures, and save them in the `data/images` directory.
- Adjust `number_images` to the desired number of images to capture.

### Label Images using LabelMe
- Open LabelMe to draw rectangles around your face for labeling.
- Set the output directory to `data/labels`.
- Label each rectangle as 'face'.

### Load Images into TensorFlow Data Pipeline
- Use TensorFlow to load and preprocess the images.

### View Raw Images
- Use Matplotlib to visualize the raw images from your dataset.

### Manually Split Data
- Move the matching labels to the appropriate train, test, and validation directories.

### Image Augmentation
- Apply various augmentations using Albumentations to enhance your dataset.

### Build and Train the Model
- Use the Functional API in TensorFlow to build and train a face detection model based on VGG16.

### Evaluate and Save the Model
- Evaluate the model on the test set and save the trained model for future use.

### Real-Time Detection
- Implement real-time face detection using your webcam.

## Important Notes
- Before running any cell, please read its comment. They contain useful information.

- To open LabelMe for labeling:

  ```sh
  !labelme
  ```

