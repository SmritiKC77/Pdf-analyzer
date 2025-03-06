**PDF Learning Resource Generator**

A Python program that scans educational PDFs and corresponding figures to automatically generate educational resources. It scans text content from PDF textbooks, analyzes images, and utilizes AI to generate organized educational materials.

**Features**

Scans text content from PDF textbooks
Analyzes and classifies figures/images using Qwen VL AI model
Generates chapter summaries with key concepts emphasized
Generates educational test items like multiple-choice, short answer, and long-answer questions
Generates Q&A files from available textbook exercises with AI-calculated answers
Associates figures with respective chapters according to content analysis

**Requirements**

Python 3.7+
Required packages: PyMuPDF (fitz), NLTK, PIL, OpenAI, python-docx, requests
OpenRouter and Qwen VL service API keys

**Usage**

from pdf_processor import main


pdf_files = ["path/to/textbook.pdf"]
figures_folder = "path/to/figures"


output_files = main(pdf_files, figures_folder)

**Output**
The tool generates up to three DOCX files:

Summary.docx: Chapter overviews with major concepts and incorporated figures

Questions.docx: Learning assessment questions with cross-references to respective figures

NCERT_Questions_Answers.docx: Current textbook questions with AI-derived answers

**Note**
The tool employs OpenRouter API to query AI models for text summarization and question preparation. Ensure proper configuration of your API keys before executing the tool.

