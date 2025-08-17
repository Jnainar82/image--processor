Image Editing with Pillow on Google Colab
This project demonstrates how to use the Pillow (PIL) library in Python to batch edit images stored in Google Drive.
The script mounts Google Drive, loads images from a specified directory, applies filters (sharpening, grayscale, smoothing), and saves the edited images to a new directory.

Features
Mounts Google Drive in Colab
Processes all images in a given folder
Applies image filters:
Sharpen → enhances edges
Grayscale (L mode) → converts to black and white
Smooth → reduces roughness
Saves edited images with a suffix _edited

Folder Setup
Before running the script, make sure you create two folders in Google Drive:
MyDrive/images → Place your original images here
MyDrive/editeding → Processed images will be saved here

Usage
Open the notebook in Google Colab.
Mount Google Drive (drive.mount('/content/drive')).
Run the script.
Find processed images inside MyDrive/editeding.

Notes
Only image files are expected in the input folder.
If re-running with different edits, delete or rename files in the output folder to avoid overwriting.
You can modify the filter pipeline (ImageFilter) to experiment with other effects.
