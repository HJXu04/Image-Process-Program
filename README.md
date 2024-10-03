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
**Launch the Program:** Run the Image Process Program.py to open the main GUI.

**Main Menu Options:**

**Add Label:** Opens a sub-window to select images, add scalebars, and labels.

**Format:** Opens a sub-window to arrange images into a grid format.

**Exit:** Click the "Quit" button in the main window or sub-windows to exit the program.
![image style="zoom:33%;"](https://github.com/user-attachments/assets/e850c5ff-ef31-4b84-9cf9-57ad829d5d37)

**Add Label and Scalebar:**
Select a folder containing images and a sample image for scalebar detection.
Configure label size, position, scale, unit, and color.
Click "OK" to process and save all images with added labels and scalebars.
![image](https://github.com/user-attachments/assets/c7b6c415-4554-4520-8564-c6b030b04fd3)
**Notes:**
1. The selected folder should contain the images of the label and scalebar to be added.
2. Sample images should contain scale information and the scale color cannot be the same as the image color. The default scale color of the program is white, which can be changed as needed.
3. The position of the label can be adjusted in pixels.
4. The transparency and color of the scalebar background box can be adjusted.
5. If you only need the scale and not the values, check the corresponding box.
**For questions about scale bar, see: https://pypi.org/project/matplotlib-scalebar**

**Image Arrangement:**
Load images from a folder and select images to arrange.
Input the number of rows and columns for the grid.
Optionally, designate an image to be enlarged and specify its grid coordinates.
Preview and save the arranged images.
![image](https://github.com/user-attachments/assets/c22a62bb-f207-422a-9926-b818ea01de65)
**Notes:**
1. You need to select an image file and set it to enlarged image.
2. The input (a,b),(c,d) coordinates indicate the area occupied by the enlarged image in the image matrix, separated by “,”.
3. If you don't want to enlarge any image, you can just let a=b=c=d.
4. You can drag the file names in the list to sort the images and click "preview" to see the preview image. If satisfied, click "save" to save.
