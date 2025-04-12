# Extraction-LLM
# Text Extraction & Financial Story Generation

This project extracts text from images/PDFs using OCR (Tesseract) and generates a financial story using Hugging Face's Phi-2 model.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Model Information](#model-information)

## Installation

1. **Install system dependencies**:
    ```bash
    !apt-get install -y tesseract-ocr poppler-utils
    ```

2. **Install Python dependencies**:
    ```bash
    !pip install pytesseract pdf2image transformers torch accelerate opencv-python matplotlib
    ```

3. **Hugging Face Authentication**:
    ```python
    from huggingface_hub import login
    login("<your_token_here>")
    ```

## Usage

### 1. Upload & Process File
Upload an image or PDF. PDFs are converted to images.
```python
def upload_and_convert():
    # Uploads file and converts PDF to images
```
## 2. OCR Preprocessing
### Preprocess the image for better OCR performance.

```
def preprocess_image_for_ocr(image_path):
    # Converts image to grayscale and applies thresholding
```
## 3. Extract Text
### Use Tesseract OCR to extract text from the image.

```
def extract_text(image_path):
    # Extracts text using pytesseract
```
## 4. Optional: Draw Bounding Boxes
### Highlight detected text regions in the image.

```
def draw_bounding_boxes(image_path):
    # Draws bounding boxes around detected text
```
## 5. Generate Financial Story
### Generate a financial narrative using the Phi-2 model.

```
def generate_financial_story(text):
    # Generates a financial story from the extracted text
```
# Model Information
## Model: microsoft/phi-2

### Library: Hugging Face Transformers

Use: Generates financial narratives from extracted text.
