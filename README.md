---

# Sudoku Digits Recognition

This project is a Python script that extracts and recognizes digits from a Sudoku puzzle image. It uses image processing techniques with OpenCV and Optical Character Recognition (OCR) with Tesseract to identify the numbers in the Sudoku grid.

---

## Features

- **Image Preprocessing**: Converts the input image to grayscale, applies Gaussian blur, and uses adaptive thresholding to prepare the image for digit extraction.
- **Grid Detection**: Identifies the Sudoku grid in the image and crops it.
- **Cell Extraction**: Divides the Sudoku grid into 81 individual cells and preprocesses each cell for digit recognition.
- **Digit Recognition**: Uses Tesseract OCR to recognize digits in each cell.
- **Output**: Displays the recognized Sudoku grid in a well-formatted 9x9 layout.

---

## Requirements

To run this project, you need the following Python libraries:

- `opencv-python`
- `pytesseract`
- `numpy`

You also need to install **Tesseract OCR** on your system. Follow the installation instructions for your operating system:
- [Tesseract Installation Guide](https://github.com/tesseract-ocr/tesseract)

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Matiin-heidari/sudoku-digit-recognition.git
   cd sudoku-digits-recognition
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure Tesseract is installed and accessible in your system's PATH.

---

## Usage

Run the script with the following command:

```bash
python sudoku_recognition.py --image path/to/your/sudoku_image.jpg
```

Replace `path/to/your/sudoku_image.jpg` with the path to your Sudoku puzzle image.

---

## Example Output

For an input Sudoku image, the script will output the recognized grid in the following format:

```
Sudoku Grid:
 5  3    |     7    |
 6       |  1  9  5 |
    9  8 |          |     6
--------------------------------
 8       |     6    |        3
 4       |  8     3 |        1
 7       |     2    |        6
--------------------------------
    6    |          |  2  8
         |  4  1  9 |        5
         |     8    |     7  9
```

---

## Notes

- The script assumes the Sudoku grid is clearly visible in the input image.
- For best results, use high-quality images with minimal noise and distortion.
- If the OCR misinterprets some digits, consider preprocessing the image further or training a custom OCR model.


---
