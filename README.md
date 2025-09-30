PDF to PPT Converter

Turn your PDFs into stunning PowerPoint presentations with ease! This Python-based Streamlit app converts multiple PDFs (like PDF0.pdf to PDF10.pdf) into a single, beautifully organized PPTX file, sorted in chronological order based on filenames. Perfect for students, professionals, or anyone needing quick, high-quality presentation slides!
Overview
The PDF to PPT Converter is a lightweight, open-source tool that transforms multiple PDFs into a PowerPoint presentation. Each PDF page becomes a slide, rendered as a high-quality image (300 DPI) in a widescreen (16:9) format. The app automatically sorts PDFs by numerical order in filenames (e.g., PDF0.pdf comes before PDF10.pdf), making it ideal for creating ordered slide decks from sequentially named files.
Installation
Get started in minutes on your Windows PC:

Prerequisites: Python 3.8+ installed (download from python.org).
Open a terminal in your project folder (e.g., C:\Users\rasha_ejuf17z\Downloads\2.Personal\PDF_PPTX).
(Optional) Create a virtual environment:python -m venv venv
venv\Scripts\activate


Install dependencies:pip install streamlit pymupdf python-pptx pillow


Copy pdf_to_ppt.py into your folder (available in this repository).

Usage

Navigate to your project folder:cd C:\Users\rasha_ejuf17z\Downloads\2.Personal\PDF_PPTX


Run the app:streamlit run pdf_to_ppt.py


Open your browser at http://localhost:8501.
Upload multiple PDFs (hold Ctrl to select multiple files, e.g., PDF0.pdf to PDF10.pdf).
Click "Convert to PPTX" and download converted.pptx.
Open the PPTX in PowerPoint to verify slides are in numerical order.

Example
Imagine you have 11 PDFs named PDF0.pdf to PDF10.pdf, each containing a single page with lecture notes. Upload all 11 files in any order, click "Convert to PPTX," and download a single PPTX with 11 slides, automatically arranged from PDF0.pdf (first slide) to PDF10.pdf (last slide). Each slide displays the PDF page as a crisp, full-size image, ready for your presentation!
Troubleshooting

Missing dependencies: Ensure all libraries are installed (pip install ...).
Large PDFs slow?: Try reducing DPI in pdf_to_ppt.py (e.g., change dpi=300 to dpi=150).
No files uploaded?: The app will show an error if you click "Convert" without selecting PDFs.
Windows path issues?: Use forward slashes or raw strings (e.g., r"C:\path\to\folder").

Contributing
Love this project? Help make it better!

Fork the repo and submit pull requests with new features (e.g., custom slide layouts, text extraction).
Report issues or suggest ideas via GitHub Issues.
Star the repo to show your support! 🌟

Join us in making PDF-to-PPT conversions effortless for everyone!
