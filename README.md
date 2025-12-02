# AI-powered-Document-Structuring-Data-Extraction-TasK
📌 Overview

This project transforms unstructured textual content from a PDF into a fully-structured Excel file using an AI (LLM)-powered key:value extraction pipeline.

The system:

Extracts raw text from Data Input.pdf

Uses an LLM to auto-detect keys (no pre-defined schema)

Preserves 100% of original wording

Outputs a clean, tabular Output.xlsx

Adds a Comments column for context

Ensures no data loss or summarization

This project was built as part of an AI internship assignment.

🚀 Features
✔ Fully automated PDF-to-Excel conversion
✔ AI detects Key : Value pairs dynamically
✔ No manual schema or hardcoded keys
✔ Comments column stores contextual sentences
✔ Guarantees 100% data capture
✔ Maintains original language and structure
✔ Works on Google Colab (recommended)
🛠 Tech Stack

Python
Google Colab
pdfplumber → PDF text extraction
LLM (OpenAI / Groq / GPT / Llama) → key:value extraction

📁 project-root/
│── main.py                     # (optional) Python script version of the notebook
│── Assignment.ipynb            # Main Google Colab notebook
│── Data Input.pdf              # Input PDF
│── Output.xlsx                 # Final generated Excel output
│── requirements.txt            # Python dependencies
│── README.md                   # Documentation (this file)

🤖 AI Extraction Logic

The LLM is instructed to:
Detect meaningful keys
Preserve original lines exactly
Place any leftover text into the Comments column
Output strict JSON format

🔍 Validation

The notebook includes a validation step that checks if every line from the PDF appears in the output.
This ensures:
No text is missing
No text is paraphrased
No data is lost

pandas → Excel creation

openpyxl → Save .xlsx file
