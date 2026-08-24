This project is an AI-powered resume parser and job description matcher built with Python. It leverages LLM APIs (Groq) along with libraries like python-docx, pypdf, and pydantic to extract structured information from resumes and compare them against job descriptions.

🚀 Features
Resume Parsing

Supports .pdf and .docx formats

Extracts candidate details: name, email, phone, skills, experiences, education, projects, certifications

Handles varied resume structures (e.g., "Experience", "Work History", "Internships")

Job Description Analysis

Converts unstructured job postings into structured JSON

Extracts role, required skills, preferred skills, education requirements, responsibilities

Candidate–Job Matching

Compares parsed resumes against job descriptions

Calculates a match score (0–100%)

Highlights matching skills, missing skills, and experience gaps

Provides a concise verdict on candidate suitability

Ranking System

Processes multiple resumes in batch

Outputs Top 2 and Lowest 2 candidates with detailed breakdowns

🛠️ Tech Stack
Python (core language)

Groq API (LLM-powered parsing & matching)

pydantic (schema validation)

python-docx (Word document parsing)

pypdf (PDF parsing)

dotenv (environment variable management)

📂 Project Structure
resume_parser.py → Main script for parsing and matching

resumes/ → Folder containing candidate resumes (.pdf / .docx)

import os.txt → Example script with job description and parsing logic

⚡ How It Works
Load job description → Convert to structured JSON

Parse resumes → Extract candidate details

Compare resume vs job → Generate match score & insights

Rank candidates → Print top and lowest matches

🔑 Setup
bash
# Clone repo
git clone https://github.com/your-username/resume-parser.git
cd resume-parser

# Create virtual environment
python -m venv .venv
source .venv/bin/activate   # Linux/Mac
.venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

# Run parser
python resume_parser.py
📊 Example Output
Code
Processing: abhay_resume.pdf
Score: 78.5
TOP 2 CANDIDATES
Abhay Singh - 78.5 %
{ "matching_skills": [...], "missing_skills": [...] }

LOWEST 2 CANDIDATES
John Doe - 42.0 %
{ "matching_skills": [...], "missing_skills": [...] }
👉 This description is ready to drop into your GitHub repo’s README.md.
Would you like me to also generate a requirements.txt file for this project so you can push it along with the repo? 
