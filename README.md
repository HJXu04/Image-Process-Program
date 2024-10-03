# Image Process Program

This application provides a graphical user interface (GUI) for processing images by adding labels and scalebars, as well as arranging and stitching images for Electron Dispersive Spectroscopy (EDS) mappings. It features two main functionalities: adding labels and scale bars to images, and arranging/stitching images into a grid format.

## Features
- **Add Label and Scale Bar**: Identify the scalebar from a sample image and automatically add it, along with a label, to all images in a specified folder.
- **Image Arrangement**: Arrange and sort selected images into a customizable grid layout with options for special image placement.
- **Graphical Interface**: Utilizes `Tkinter` to create an intuitive user interface for file selection, input, and image preview.
- **Support for Multiple Image Formats**: Works with `.png`, `.jpg`, `.jpeg`, `.bmp`, `.tif`, and `.tiff` image formats.

## Requirements
- Python 3.x
- Required Python libraries:
  - `Pillow` (for image manipulation)
  - `matplotlib` (for image visualization)
  - `matplotlib-scalebar` (for adding scalebars)
  - `Tkinter` (for GUI)

Install the required libraries with:
```bash
pip install pillow matplotlib matplotlib-scalebar
```

## How to Use
Launch the Program: Run the Image Process Program.py to open the main GUI.

Main Menu Options:

Add Label: Opens a sub-window to select images, add scalebars, and labels.
Format: Opens a sub-window to arrange images into a grid format.
Add Label and Scalebar:

Select a folder containing images and a sample image for scalebar detection.
Configure label size, position, scale, unit, and color.
Click "OK" to process and save all images with added labels and scalebars.
Image Arrangement:

Load images from a folder and select images to arrange.
Input the number of rows and columns for the grid.
Optionally, designate an image to be enlarged and specify its grid coordinates.
Preview and save the arranged images.
Exit: Click the "Quit" button in the main window or sub-windows to exit the program.
