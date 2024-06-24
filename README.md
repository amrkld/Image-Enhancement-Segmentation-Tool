# Image Enhancement/Segmentation Project

## Overview
This project is a graphical user interface (GUI) application built using Python's `tkinter` library. The application provides various image processing functionalities including histogram enhancement, Gaussian filtering, mean shift segmentation, and Gaussian adaptive thresholding. Users can open an image, apply these effects, and save the modified image.

## Features
- **Open Image:** Load an image file (supports `.png`, `.jpg`, and `.jpeg`).
- **Histogram Enhancement:** Adjust contrast and brightness by redistributing pixel intensity values.
- **Gaussian Filter:** Smooth an image by convolving it with a Gaussian kernel, reducing noise while preserving edges.
- **Mean Shift Segmentation:** Group similar pixels into clusters based on feature similarity using mean shift algorithm.
- **Gaussian Adaptive Thresholding:** Segment an image by thresholding each pixel based on the local Gaussian-weighted mean of its neighborhood.
- **Remove all effects:** Reset the image to its original state.
- **Download Image:** Save the modified image to your local machine.

## Usage
1. **Open the application:** Run the `main.py` script.
2. **Open an image:** Click on the "Open Image" button and select an image file.
3. **Apply enhancements or segmentations:** Use the available buttons to apply different effects:
   - Histogram Enhancement
   - Gaussian Filter
   - Mean Shift Segmentation
   - Gaussian Adaptive Thresholding
4. **Reset image:** Click "Remove all effects" to reset the image.
5. **Download the modified image:** Click "Download Image" to save the modified image.

## Code Structure
- `ToolTip`: A helper class to create tooltips for the buttons.
- `ImageProcessorApp`: The main application class containing:
  - `__init__`: Initializes the application, sets up the GUI components.
  - `open_image`: Opens and displays an image.
  - `display_image`: Updates the image display.
  - `Histogram_Enhancement`: Applies histogram equalization.
  - `Gaussian_Filter`: Applies Gaussian filtering.
  - `Mean_shift_Segmentation`: Applies mean shift segmentation.
  - `gaussian_threshold`: Applies Gaussian adaptive thresholding.
  - `display_modified_image`: Updates the display with the modified image.
  - `clear_canvas`: Resets the image to its original state.
  - `download_image`: Saves the modified image.

## GUI Components
- **Main window:** Contains image display and buttons for functionalities.
- **Buttons:**
  - `Open Image`: Opens an image file.
  - `Histogram Enhancement`: Applies histogram equalization.
  - `Gaussian Filter`: Applies Gaussian filtering.
  - `Mean Shift Segmentation`: Applies mean shift segmentation.
  - `Gaussian Adaptive Thresholding`: Applies Gaussian adaptive thresholding.
  - `Remove all effects`: Resets the image.
  - `Download Image`: Saves the modified image.

## Tooltips
Each button has a tooltip providing a brief description of its functionality.

## Dependencies
- `tkinter`: For the GUI.
- `PIL` (Pillow): For image handling.
- `cv2` (OpenCV): For image processing functions.
- `numpy`: For numerical operations.
- `matplotlib`: For displaying images and histograms.
- `scipy.ndimage`: For Gaussian filtering.
- `sklearn.cluster`: For mean shift segmentation.

## Notes
- Ensure all dependencies are installed before running the application.
- The application supports images with `.png`, `.jpg`, and `.jpeg` extensions.
- Tooltips provide additional guidance on the functionalities of each button.
