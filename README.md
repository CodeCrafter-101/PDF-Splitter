# PDF-Splitter


## Project Overview
- PDF Splitter is a simple Python utility that splits a PDF file into multiple smaller PDF files — either page by page or based on a custom page range. This tool is useful when you want to extract individual pages or sections from a large PDF file for sharing, editing, or archiving.

## Features
- Split every page into a separate PDF
- Extract a range of pages (e.g., pages 2–5)
- Save output files with automatic naming
- Lightweight and easy to use

## Libraries Used:
- `PyPDF2` – for PDF manipulation
- `os` – for handling files and paths

## Requirements
### pip install PyPDF2
````
pip install PyPDF2
````


## How It Works
### 1. Load the PDF File
- Read the PDF using `PyPDF2.PdfReader`
### 2. Choose Split Type
- Split all pages individually, or
- Split by a specific range (e.g., pages 3–7)
### 3. Save Output
- Save the extracted pages as new `.pdf` files

## Steps to Run
### 1. Clone the Repository
````
git clone https://github.com/CodeCrafter-101/pdf-splitter.git
cd PDF-Splitter
````
### 2. Install Dependencies
````
pip install PyPDF2
````
### 3. Set the paths
- Enter the path to your input PDF file.
- Enter the output directory where you want the split PDF files to be saved.

### 4. Run the Script
- Edit and run `split_pdf()` with your desired input PDF and page range:
````
split_pdf("sample.pdf")               # splits into separate pages
split_pdf("sample.pdf", 2, 5)         # extracts pages 2 to 5
````

## 📂 Output File Naming
- `page_1.pdf`, `page_2.pdf`, ... for full split
- `pages_2_to_5.pdf` for range-based split



