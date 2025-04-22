# Chessboard Analysis: AI & Computer Vision

## Content 
 Technologies & Libraries Used
 Algorithm & Steps
 How to Run in Google Colab
 Test & Validation
 
## Technologies & Libraries Used:-
Python (Programming Language)

OpenCV (cv2): For image processing and computer vision tasks.

NumPy: For mathematical operations on image data.

Matplotlib: For displaying images in the Colab notebook.

Google Colab: Platform to run the solution interactively in the browser.

## *Input*- 
Upload a clear image of a standard chessboard (8x8 squares). The image should be well-lit and not overly distorted.

## Algorithm & Steps:-
### Image Upload:

Uses google.colab.files.upload() to allow manual image uploads in Colab.

Loads the image using cv2.imread().

### Preprocessing:

Converts the image to grayscale (simplifies processing).

Applies Gaussian blur to reduce noise.

Uses adaptive thresholding to handle uneven lighting.

### Chessboard Detection:

Uses cv2.findChessboardCorners() to locate the corners in a standard 7x7 grid pattern.

If successful, the corners are drawn using cv2.drawChessboardCorners().

### Counting Squares:

Based on the known 8×8 layout, the bounding box around detected corners is divided into grid cells.

Each square is classified as black or white using the index (i+j) % 2 pattern.

Annotated with colors to help visualize correctness.

### Output:

Displays the image with rectangles drawn around each square.

Prints total black and white square counts.

### Output Example: 
Chessboard Square Count:
Black Squares: 32
White Squares: 32

## How to Run in Google Colab:-
Open the notebook in Google Colab.

Run each cell in sequence.

When prompted, upload a clear chessboard image (top view preferred).

The notebook will process and show:

Detected corners

Annotated grid

Count of black and white squares.

## Test & Validation:-
Tested on two chessboard images with:

Different angles

Slight shadows

Skewed alignment



## Bonus-
This solution is extendable to detect non-standard boards (like partial boards) by tweaking the grid size in cv2.findChessboardCorners() and adjusting the bounding logic.
