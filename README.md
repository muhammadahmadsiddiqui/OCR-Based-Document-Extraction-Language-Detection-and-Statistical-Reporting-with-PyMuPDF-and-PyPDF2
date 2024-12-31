# OCR-Based Document Extraction, Language Detection, and Statistical Reporting with PyMuPDF and PyPDF2

## Overview

This project provides a comprehensive solution for extracting text from documents, detecting the language of the text, and performing statistical analysis such as word count and confidence intervals. It supports multiple document formats, including PDF and MSG files, and uses Optical Character Recognition (OCR) for extracting text from scanned PDFs or images. The implementation also includes statistical analysis on the word count of document contents, using methods such as mean, standard error, and bootstrap confidence intervals.

## Features

- **Text Extraction from PDFs and MSG Files**:
  - Direct text extraction from PDF files using PyPDF2.
  - Optical Character Recognition (OCR) using PyMuPDF and pytesseract for PDFs with images or scanned content.
  - Text extraction from `.msg` email files using `extract_msg`.
  
- **Language Detection**:
  - Language detection for extracted text using the `langdetect` library.
  
- **Statistical Reporting**:
  - Word count analysis for each document.
  - Calculation of the mean word count across documents.
  - Statistical reporting including 95% confidence intervals using `scipy.stats` and bootstrap methods.

- **JSON Output**:
  - Saves the extracted data, including document content, language detection, and statistical results to a JSON file.

## Prerequisites

Before running the script, ensure the following dependencies are installed. See the provided `requirements.txt` file to install all necessary libraries.

### Installation

1. Clone or download this repository.
2. Create a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
