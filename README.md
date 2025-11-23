# Nirmaan AI Intern Case Study Solution

This tool analyzes student self-introductions based on a transcript and produces a rubric-based score (0-100).

## Features
- **Rule-based:** Checks for keywords, specific salutations, and flow.
- [cite_start]**NLP-based:** Uses `sentence-transformers` for semantic meaning and `spacy` for linguistic analysis[cite: 18].
- [cite_start]**Data-driven:** Strictly follows the weighting and scoring formulas provided in the Case Study Rubric Excel file[cite: 19].

## Prerequisites
- Python 3.8 or higher
- Java (Required for `language-tool-python`)

## [cite_start]Installation & Local Deployment [cite: 37]

1. **Clone or Download this repository.**
2. **Install dependencies:**
   Open your terminal/command prompt in this folder and run:
   ```bash
   pip install -r requirements.txt