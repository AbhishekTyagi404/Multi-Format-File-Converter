# Multi-Format File Converter

## Overview
This project is a **multi-format file converter** that allows users to convert files between various formats including **PDF, DOCX, TXT, PPTX, and images (JPG/PNG)**. It is built using **Flask** and provides a simple web-based interface for file conversion.

## Features
- **PDF to DOCX**
- **DOCX to PDF** (via HTML conversion for Unicode support)
- **TXT to PDF/DOCX**
- **PPTX to PDF** (supports Hindi and Unicode)
- **Image (JPG/PNG) to PDF**
- **Auto file cleanup** (removes uploaded and converted files after 30 minutes)

## Tech Stack
- **Backend:** Flask (Python)
- **Frontend:** Bootstrap (HTML, CSS, JS)
- **Libraries Used:**
  - `Flask`
  - `pdf2docx`
  - `fpdf`
  - `PIL` (Pillow)
  - `docx`
  - `pypandoc`
  - `werkzeug`
  - `pptx`

## Installation

### Prerequisites
Make sure you have Python 3.8+ installed.

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/multi-format-file-converter.git
   cd multi-format-file-converter
   ```

2. Create and activate a virtual environment:
   ```sh
   python3 -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

4. Ensure Pandoc is installed:
   ```sh
   sudo apt install pandoc
   ```
   Or manually install it from [Pandoc's official site](https://pandoc.org/).

5. Start the Flask app:
   ```sh
   python converter.py
   ```

6. Open the browser and go to:
   ```
   http://127.0.0.1:5000/
   ```

## Usage
1. Upload a file.
2. Select the desired conversion format.
3. Click "Convert" and download the converted file.

## Auto File Cleanup
A background process runs every **30 minutes** to delete old files automatically.

## Contributing
Feel free to fork this repository, make improvements, and submit a pull request.

## License
This project is licensed under the MIT License.

## Contact
For any issues or suggestions, feel free to reach out via GitHub Issues.🚀
