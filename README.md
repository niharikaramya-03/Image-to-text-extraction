# Image to Text Extraction using Optical Character Recognition (OCR)

This project is a simple Flask web application that extracts text from uploaded images using **Tesseract OCR**. It demonstrates a practical application of image processing and text recognition using Python.

---

# Features

- Upload image files through a web interface
- Extracts text from images using Tesseract OCR
- Displays extracted text instantly
- Sample images included for testing

---

# Tech Stack

- **Python**
- **Flask** for web application
- **Tesseract OCR** for text recognition
- **pytesseract** (Python wrapper)
- **OpenCV**, **Pillow**, and **NumPy**

---

# Project Structure
app/
│ ├── app.py # Main Flask app
│ ├── config.py # Configuration settings
│ ├── static/uploads/ # Folder to store uploaded images
│ └── templates/ # HTML templates
├── Optical_Character_Recognition_using_Image.ipynb # Jupyter Notebook demo
├── requirements.txt # Dependencies list
├── Procfile # Deployment configuration
└── readme.md # Project documentation

---

## ⚙️ Installation & Setup

### ✅ Prerequisites

- Python 3.6+
- Tesseract OCR installed on your system  
  📥 [Windows Installer](https://github.com/UB-Mannheim/tesseract/wiki)

### 💻 Steps to Run Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/image-to-text-ocr.git
   cd image-to-text-ocr
   
2. **Create a Virtual Environment**
   ```bash
   conda create -n ocr-env python=3.8
   conda activate ocr-env

3. **Install Python Requirements**
   ```bash
   pip install -r requirements.txt

4. Install Tesseract

Download and install Tesseract from the link above
Note the installation path (e.g., C:\Program Files\Tesseract-OCR\tesseract.exe)

5. Set Tesseract Path
In your Python code (or globally), set:
   ```bash
   pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'

6. Run the App
    python app.py

7. Open in Browser
Navigate to: http://127.0.0.1:5000/

## Sample Data
Test images are available in the sample_data/ directory for quick verification.

## Deployment
Includes Procfile for deployment on platforms like Heroku.
Make sure to configure Tesseract OCR in your deployment environment.

## Future Improvements
Language selection support

PDF and multi-page image support

Improved UI and mobile responsiveness

Drag and drop image upload
