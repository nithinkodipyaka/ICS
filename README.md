# Intelligent Campus Surveillance (ICS)

## Overview
The Intelligent Campus Surveillance (ICS) project is designed to enhance campus security by utilizing computer vision techniques for face recognition and ID card detection. The project includes the following functionalities:

1. **Face Recognition:** The system can recognize and identify known individuals by comparing their facial features with pre-registered face encodings.

2. **Live CCTV Feed Processing:** The system processes live CCTV feed, detects faces, compares them with known encodings, and saves images of recognized individuals.

3. **ID Card Detection:** The project includes a module to detect and identify ID cards or lanyards in the saved images from the live CCTV feed.

## Project Structure

### 1. `face_segmentation.ipynb`
This file contains utility functions for face recognition, including the creation and comparison of face encodings.

### 2. `cctv_processing`
This script processes the live CCTV feed, performs face recognition, and saves images of recognized individuals to a directory.

### 3. `IDtag_detection.ipynb`
This script integrates with the Roboflow platform to detect and identify ID cards or lanyards in the saved images.

### 4. `ICS.ipynb`
The main script orchestrates the entire project. It loads known face encodings, processes live CCTV feed, saves recognized faces, and detects ID cards.

## Instructions for Use

1. **Install Dependencies:** Make sure you have the required dependencies installed. You can install them using: `pip install opencv-python roboflow`

2. **Set Up Known People Images:**
- Place individual images of known people in the `Facedata/People` directory. Each image should contain only one face.
- Run the `processKnownPeopleImages` function in `ICS.ipynb` to create and save face encodings for known people.

3. **Run the Main Script:**
- Execute the `ICS.ipynb` script to start the face recognition and live CCTV feed processing.

4. **ID Card Detection:**
- The script also integrates with the Roboflow platform to detect and identify ID cards or lanyards in the saved images from the live CCTV feed.

5. **Results:**
- The processed images with recognized faces and detected ID cards will be saved in the `Facedata/saved_img<name>` directory.

## Notes
- The project is designed for educational purposes and may require customization for specific use cases.
- Ensure that the file paths and dependencies are configured correctly based on your environment.

## License
This project is licensed under the terms of the LICENSE file.

## Copyright
© 2023 Nithin Kodipyaka


