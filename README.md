# Image Processing on Image Dataset

## Overview
This project demonstrates the application of fundamental image processing techniques using OpenCV. We work on a set of images and perform various enhancements and feature extraction operations.

Dataset used: [Animal Images Classification Dataset](https://www.kaggle.com/code/drisrarahmad/animal-images-classification-dataset)

---

## Objectives
- Adjust brightness and contrast
- Apply Gaussian blur for smoothing
- Detect edges using the Canny algorithm
- Reduce noise in the images
- Extract ORB (Oriented FAST and Rotated BRIEF) features

---

## Folder Structure
```
project/
├── main.py                     # main execution file
├── processed_images/          # stores the output results
├── README.md                  # this file
```

---

## Requirements
- Python 3.x
- OpenCV
- NumPy
- Matplotlib

Install requirements with:
```bash
pip install opencv-python numpy matplotlib
```

---

## How to Run

1. Download the dataset from Kaggle.
2. Extract the dataset and set the correct path in `main.py` or in Colab cell.
3. Run the script using:
 run all cells in order.

- The first 5 images from the dataset will be processed.
- Each step (adjustment, blur, edge, noise removal, features) will be visualized separately.
- Output images will be saved in a folder named `processed_images`.

---

## Sample Results

| Step                | Description                   |
|---------------------|-------------------------------|
| Brightness & Contrast | Enhanced image visibility    |
| Gaussian Blur         | Smoother image, less noise   |
| Canny Edge Detection  | Clear edges and outlines     |
| ORB Features          | Keypoints drawn on image     |

---

# limitations

Limited Number of Images: The script processes only the first 5 images from the dataset for demonstration purposes. You can increase this by modifying max_images in the code.

Fixed Parameters: Brightness, contrast, and thresholds in filters are hardcoded. Dynamic tuning or user input is not implemented yet.

Basic Exception Handling: The script handles common errors (like missing or unreadable images), but doesn't cover all edge cases (e.g., corrupted image files, unreadable directories).

No Batch Output Comparison: Processed results are shown and saved individually per image. There's no combined comparison grid or report summary yet.

---
## Notes
- All exceptions (e.g., corrupted images or missing files) are handled gracefully.
- Modify `max_images` in the code to process more images.

---

