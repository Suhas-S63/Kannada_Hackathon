# Kannada OCR and Writer Identification Project
---

## Team Members
- **Suhas S**
- **Sai Darshan**
- **Guhan KS**
--- 

## Overview

This project was developed as part of the "Kannada Hackathon," focusing on enhancing technology for the Kannada language. The primary objective is to improve text extraction from images and PDF files using advanced Optical Character Recognition (OCR) techniques, as well as implement innovative solutions such as writer identification and keyword search for Kannada texts.

### Key Features:
- **Image to Text Extraction**: Developed an advanced OCR system capable of extracting text from Kannada images, leveraging machine learning techniques to enhance accuracy and efficiency.
- **Writer Identification**: Designed a system to identify the authors of Kannada manuscripts and handwritten texts using VGG16 CNN architecture.
- **Keyword Search**: Implemented a keyword search functionality for Kannada text files, allowing custom searches within large volumes of text.

---

## Project Flow

1. **Input Handling**:
   - Extract images from PDFs using `PyMuPDF`.
   - Load and preprocess images (invert colors, sharpen, apply binary thresholding).

2. **Image Preprocessing**:
   - Enhance image quality for OCR by applying sharpening filters and thresholding.
   - Crop images based on detected rows and columns of text.
   - Remove duplicate cropped images using Structural Similarity Index (SSIM).

3. **OCR Process**:
   - Choose between three OCR engines: Tesseract, EasyOCR, and PaddleOCR.
   - Extract Kannada and English text from preprocessed images.

4. **Text Output**:
   - Save extracted text to organized directories in `.txt` files.
   - Option to append or overwrite OCR results based on user requirements.

---

## Hackathon Initiatives

### Image to Text Extraction
We developed a powerful OCR system that extracts Kannada text from images using machine learning models like Convolutional Neural Networks (CNNs). The system enhances both accuracy and efficiency, helping streamline the process of converting images into text files.

### Writer Identification
In addition to OCR, we designed a writer identification system for Kannada manuscripts and handwritten documents. This project utilizes the VGG16 CNN architecture to analyze handwriting features and classify authors based on their unique writing style.

- **Applications**:  
  - Forensic analysis: Identifying authors in criminal investigations.  
  - Historical research: Analyzing historical Kannada manuscripts.  
  - Education: Providing personalized feedback on handwriting.

### Keyword Search
We implemented a keyword search functionality for Kannada text files. Users can easily conduct custom searches, making it faster and easier to find specific information within large volumes of text.

---

## Installation

To run this project, install the required Python packages by running the following command:

```bash
pip install -r requirements.txt
```

### Required Packages:
- `opencv-python`
- `PyMuPDF`
- `pytesseract`
- `easyocr`
- `paddleocr`
- `scikit-image`
- `numpy`

---

## Usage

To run the project, provide the path to the input file (PDF or image) and specify the OCR engine to use.

### Example:

```bash
python main.py --file_path /path/to/your/image_or_pdf --model_type easyocr
```

Available OCR models:
- `tesseract`
- `easyocr`
- `paddleocr`

---

## Directory Structure

```
project_root/
│
├── output/
│   ├── pdf_images/        # Extracted images from PDF
│   ├── preprocessed_images/  # Preprocessed images for OCR
│   ├── cropped_images/    # Cropped images based on rows and columns
│   └── ocr_texts/         # Extracted text saved as .txt files
│
├── main.py                # Main script for running the OCR process
└── requirements.txt       # Python packages to install
```

---

## Commitment to Kannada Development

This project reflects our dedication to advancing the Kannada language through technology. Our initiatives not only promote the growth of Kannada but also preserve its cultural heritage. By integrating state-of-the-art tools and techniques, we are creating resources that can significantly benefit the Kannada-speaking community.


---

## Future Improvements
- **Improved OCR Accuracy**: Further refining image preprocessing techniques for better accuracy in low-quality documents.
- **GUI Interface**: Developing a user-friendly interface to make the process more accessible.
- **Language Expansion**: Extending support to additional Indian languages.

---

## License

This project is open-source and available under the MIT License.

---

## Acknowledgments

Special thanks to the hackathon organizers and the open-source community for their contributions to the libraries and tools used in this project.
```

This markdown file includes the entire project description, highlights the hackathon initiatives, and lists the team members. It provides a clear and readable structure for anyone interested in your project.
