# Image Processing with OpenCV and Matplotlib

This notebook demonstrates basic image processing operations using OpenCV and Matplotlib in Python. The script processes image files in different formats (JPG, PNG, TIFF) by converting them to RGB and grayscale, displaying histograms, and saving the results in multiple formats.

## Requirements

The following packages are required:
- Python 3.x
- OpenCV (`cv2`)
- Matplotlib
- NumPy
- Jupyter Notebook
- Pillow

### Installation

You can install all required packages using the provided `requirements.txt` file:

```bash
pip install -r requirements.txt
```

## Directory Structure

The script expects the following directory structure:

```
.
├── requirements.txt
├── image_processing.ipynb
├── img/
│   ├── jpg/
│   │   └── result/
│   ├── png/
│   │   └── result/
│   └── tiff/
│       └── result/
```

Place your images in the `img/` directory or in the respective format subdirectories.

## How It Works

1. **Image Detection**: The script searches for JPG, PNG, and TIFF images in the main directory and format-specific subdirectories.

2. **Image Processing**: For each image found, the script performs the following operations:
   - Converts the image to RGB color space
   - Converts the image to grayscale
   - Displays the RGB and grayscale versions
   - Generates and displays color histograms

3. **Cross-Format Conversion**: The script saves each processed image in all three formats (JPG, PNG, TIFF) in their respective result directories.

## Usage

1. Install required packages: `pip install -r requirements.txt`
2. Launch Jupyter Notebook: `jupyter notebook`
3. Open the `image_processing.ipynb` file
4. Ensure your images are in the correct directories
5. Run the notebook cells in sequence
6. Processed images will be saved in the `result` subdirectories of each format directory

## Code Overview

The main steps in the code are:

1. Setting up directory paths
2. Finding all image files
3. Processing each image:
   - Reading the image
   - Converting to RGB and grayscale
   - Displaying the images and histograms
   - Saving in different formats

## Example Output

For each image processed, you will see:
- An RGB visualization
- A grayscale visualization
- A color histogram showing the distribution of pixel intensities

## Notes

- The script automatically creates necessary directories if they don't exist.
- If an image cannot be read, the script will print an error message and continue with the next image.
- The histogram is displayed but not saved as an image file.