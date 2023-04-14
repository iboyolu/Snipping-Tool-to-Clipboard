# Windows Snipping Tool OCR

This Python script automatically converts images copied from the Windows Snipping Tool into text and copies the text to the clipboard. The script uses the Tesseract OCR engine and the Pytesseract library to perform optical character recognition on the image.

## Requirements

- Python 3.11.3 or later
- Tesseract OCR engine
- Pytesseract library
- PIL library
- Pyperclip library

## Installation

1. Install Python 3.11.3 or later from the official Python website.
2. Install Tesseract OCR engine. You can download the installer for Tesseract OCR from the [official website](https://github.com/UB-Mannheim/tesseract/wiki). Make sure to add Tesseract OCR to your system's PATH environment variable.
3. Install the required Python libraries by running the following command in your terminal or command prompt:

```pip install pytesseract pillow pyperclip```


4. Download or clone this repository to your local machine.

## Usage

1. Open the Windows Snipping Tool and capture an image.
2. Copy the image to the clipboard by pressing `Ctrl+C` or clicking the "Copy" button in the Snipping Tool.
3. Run the `snipping_tool_ocr.py` script by running the following command in your terminal or command prompt:

```python snipping_tool_ocr.py```


4. The script will automatically convert the image to text and copy the text to the clipboard.
5. Paste the text into your desired application by pressing `Ctrl+V` or right-clicking and selecting "Paste".

## Customization

You can customize the script to fit your needs by modifying the following variables:

- `LANG`: The language of the text in the image. The default value is `'eng'` for English. You can change this to any language supported by Tesseract OCR.
- `PSM`: The page segmentation mode used by Tesseract OCR. The default value is `6`, which assumes a single uniform block of vertically aligned text of uniform font. You can change this to any value supported by Tesseract OCR.
- `OEM`: The OCR Engine Mode used by Tesseract OCR. The default value is `1`, which uses the LSTM OCR engine. You can change this to `0` to use the original Tesseract OCR engine.

## Known Issues

- The script may not work with images that contain handwriting or non-standard fonts.
- The script may not work with images that have low contrast or are blurry.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
