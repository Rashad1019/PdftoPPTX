# PDF to PPT Converter

Create stunning PowerPoint presentations from PDFs instantly!

👉 **[Use the App Online](https://pdftopresentation.streamlit.app/)**

This tool converts multiple PDFs into a single PPTX file, sorted by numerical filename order. Perfect for **students, educators, and professionals** who want fast, clean slide decks from their documents.

---

## 🚀 Overview

The **PDF to PPT Converter** is a Python-based [Streamlit](https://streamlit.io/) app that transforms multiple PDFs into a PowerPoint presentation.

* Each PDF page becomes a **widescreen (16:9) slide** with a high-quality image (**300 DPI**).
* Files are **automatically sorted numerically** by filename (e.g., `Note_1.pdf` comes before `Note_10.pdf`).
* Works both **online** and **locally**.

---

## 🛠 Installation (Local Setup)

Run the app on your Windows PC:

1. **Install Python 3.8+**
   Download from [python.org](https://www.python.org/downloads/) and check “Add Python to PATH.”

2. **Clone or create a folder**

   ```bash
   git clone https://github.com/yourusername/pdf-to-ppt-converter.git
   cd pdf-to-ppt-converter
   ```

3. **(Optional) Create a virtual environment**

   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

4. **Install dependencies**

   ```bash
   pip install streamlit pymupdf python-pptx pillow
   ```

5. **Add code**
   Place `pdf_to_ppt.py` into the folder (or use the repo copy).

---

## 📖 Usage

### Online (recommended)

👉 [Launch the app here](https://pdftopresentation.streamlit.app/)

1. Upload multiple PDFs (hold **Ctrl** to select).
2. Click **Convert to PPTX**.
3. Download the generated `converted.pptx`.

### Local

```bash
streamlit run pdf_to_ppt.py
```

Then open the local URL (e.g., `http://localhost:8501`) in your browser.

---

## 🎯 Example

Upload a set of PDFs (e.g., meeting notes):

* The app sorts them by filename numbers.
* Each page is converted into a **clear, high-resolution slide**.
* Result: A presentation ready for use in **PowerPoint, Google Slides, or Keynote**.

---

## 🐛 Troubleshooting

* **Missing dependencies?**

  ```bash
  pip install streamlit pymupdf python-pptx pillow
  ```

* **Slow conversion?**
  Edit `pdf_to_ppt.py` → set `dpi=150`.

* **No PDFs uploaded?**
  App shows an error if "Convert" is clicked without files.

---

## 🤝 Contributing

Want to make this better?

* Fork and submit **pull requests** (e.g., add slide templates).
* Report issues via **GitHub Issues**.
* ⭐ Star the repo to support the project!
