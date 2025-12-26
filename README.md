# 🧠 LangChain Resume Analyzer & CSV Generator

An LLM-powered resume processing system that automatically extracts structured candidate information from bulk resumes (PDF/DOCX) and converts them into a clean, downloadable CSV file for easy analysis.

This project leverages LangChain + Google Gemini to transform unstructured resume data into HR-ready structured datasets with high accuracy.

## 🚀 Project Overview

Recruiters and data teams often receive resumes in unstructured formats that are difficult to analyze at scale.
This project solves that problem by:

Accepting a ZIP file of resumes

Automatically parsing each resume using an LLM

Extracting standardized candidate fields

Generating a CSV file for downstream analytics, filtering, or ATS ingestion

## ✨ Key Features

### 📦 Bulk Resume Upload (ZIP file support)

### 📄 Supports PDF & DOCX resume formats

### 🧠 LLM-driven semantic extraction using LangChain

### 📊 Converts resumes into structured CSV

### ⚙️ Schema-enforced output using Pydantic

### 🔍 Live data preview inside Streamlit

### ⬇️ One-click CSV download

##📚 Extracted Resume Fields

Each resume is parsed into the following structured fields:

1. Full Name

2. Email Address

3. Phone Number

4. Technical Skills

5. Experience Summary

6. Education Details

7. LinkedIn Profile

8. GitHub Profile

## 🛠️ Tech Stack

1. Streamlit – Interactive UI

2. LangChain – LLM orchestration

3. Google Gemini (2.5 Flash) – Resume understanding

4. Pydantic – Schema validation

5. PyPDF2 – PDF text extraction

6. CSV – Structured output generation
  
7. python-docx – DOCX parsing

## 🧩 How It Works

1. Upload a ZIP file containing resumes

2. Resumes are extracted and read (PDF/DOCX)

3. Text is passed to a LangChain + Gemini pipeline

4. Output is validated against a strict schema

5. All resumes are merged into a single CSV file

6. CSV is made available for download and preview

## ⚙️ Setup Instructions
```
# 1. Clone the repository
git clone https://github.com/your-username/langchain-resume-analyzer.git
cd langchain-resume-analyzer

# 2. Create and activate virtual environment
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r req.txt

# 4. Add API key
# Create a .env file
GOOGLE_API_KEY=your_google_gemini_api_key

# 5. Run the app
streamlit run main.py
```

## 📈 Use Cases

1. HR Resume Screening Automation

2. Candidate Database Creation

3. Talent Analytics & Reporting

4. ATS Pre-processing

5. AI-powered Resume Mining

## 🧪 Tested & Verified

✔ End-to-end tested with multiple resume formats
✔ Handles noisy/unstructured resume text
✔ Produces consistent schema-aligned output

## 📄 Project Structure
├── main.py        # Streamlit application logic
├── req.txt        # Dependencies
├── .env           # API key configuration

## 🙌 Acknowledgements

Built using LangChain and Google Gemini to demonstrate real-world LLM applications in HR automation and unstructured data transformation.
