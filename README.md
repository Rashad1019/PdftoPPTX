# PDF to PPT Converter

Transform your PDFs into stunning PowerPoint presentations in a snap! This Python-based Streamlit app converts multiple PDFs (like PDF0.pdf to PDF10.pdf) into a single, beautifully organized PPTX file, sorted in chronological order by filename. Perfect for students, professionals, or anyone needing quick, high-quality slides!

## Overview
The PDF to PPT Converter is a lightweight, open-source tool that turns multiple PDFs into a PowerPoint presentation. Each PDF page becomes a slide, rendered as a high-quality image (300 DPI) in a widescreen (16:9) format. The app automatically sorts PDFs by numerical order in filenames (e.g., PDF0.pdf before PDF10.pdf), making it ideal for creating ordered slide decks from sequentially named files.

## Installation
Set up the app on your Windows PC with these steps:

1. **Install Python 3.8+**: Download from [python.org](https://python.org) and ensure "Add Python to PATH" is checked.

2. **Set up project folder**: Use `C:\Users\rasha_ejuf17z\Downloads\2.Personal\PDF_PPTX` or create a new folder.

3. **(Optional) Create a virtual environment**:
   ```bash
   cd C:\Users\rasha_ejuf17z\Downloads\2.Personal\PDF_PPTX
   python -m venv venv
   venv\Scripts\activate
   ```

4. **Install dependencies**:
   ```bash
   pip install streamlit pymupdf python-pptx pillow
   ```

5. **Add the app code**: Copy `pdf_to_ppt.py` from this repository into your folder.

## Usage

1. **Navigate to your project folder**:
   ```bash
   cd C:\Users\rasha_ejuf17z\Downloads\2.Personal\PDF_PPTX
   ```

2. **Run the app**:
   ```bash
   streamlit run pdf_to_ppt.py
   ```

3. **Open your browser** at http://localhost:8501.

4. **Upload multiple PDFs** (hold Ctrl to select files, e.g., PDF0.pdf to PDF10.pdf).

5. **Click "Convert to PPTX"** and download `converted.pptx`.

6. **Open the PPTX in PowerPoint** to verify slides are in numerical order.

## Example
Got 11 PDFs named PDF0.pdf to PDF10.pdf with lecture notes? Upload them in any order, click "Convert to PPTX," and get a single PPTX with 11 slides, automatically arranged from PDF0.pdf (first slide) to PDF10.pdf (last slide). Each slide shows the PDF page as a crisp, full-size image, ready for your next presentation!

## Troubleshooting

- **Missing dependencies?** Run `pip install streamlit pymupdf python-pptx pillow` again.
- **Slow with large PDFs?** Edit `pdf_to_ppt.py` to lower DPI (e.g., change `dpi=300` to `dpi=150`).
- **No files uploaded?** The app will show an error if you click "Convert" without selecting PDFs.
- **Path issues on Windows?** Use forward slashes or raw strings (e.g., `r"C:\path\to\folder"`).

## Contributing
Love this project? Help make it awesome!

- Fork the repo and submit pull requests with features (e.g., custom slide layouts, text extraction).
- Report bugs or suggest ideas via GitHub Issues.
- Star the repo to spread the word! 🌟

Join us in making PDF-to-PPT conversions effortless for everyone!