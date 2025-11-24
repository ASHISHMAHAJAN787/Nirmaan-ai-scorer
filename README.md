# 🎙️ Nirmaan AI Communication Scorer

### Automated Spoken Communication Assessment Tool
*Developed for Nirmaan Organization AI Intern Case Study*

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)

## 📋 Project Overview
This tool is an AI-powered grading system designed to analyze student self-introductions. It accepts a text transcript and audio duration as input, processes the content using various NLP techniques, and generates a **rubric-based score (0-100)** with detailed feedback.

The solution combines **Rule-based logic**, **Semantic NLP (Sentence Transformers)**, and **Grammar Analysis** to provide a holistic assessment of communication skills.

---

## 🚀 Live Demo
- **Deployed App:** [https://nirmaan-ai-scorer-by-ashish-mahajan.streamlit.app/]
- **Demo Video:** [https://drive.google.com/drive/folders/1pAZxAKzMl4b1btwwsPR174nhTpAoZ4KH?usp=drive_link]

---

## 🛠️ Features & Scoring Logic
The scoring system is strictly data-driven based on the provided Case Study Rubric.

| Criterion | Weight | Method / Formula |
|-----------|--------|------------------|
| **Salutation** | 5% | **Rule-based:** Checks for formal greetings (e.g., "Good Morning" vs "Hi"). |
| **Keyword Presence** | 30% | **Semantic NLP:** Uses `sentence-transformers` to find semantic matches for mandatory details (Name, Age, Family) and optional details (Ambition, Hobbies). |
| **Flow** | 5% | **Logic-based:** Verifies the structural order: Salutation → Name → Closing. |
| **Speech Rate** | 10% | **Math:** Calculates Words Per Minute (WPM). Ideal range: 111-140 WPM. |
| **Grammar** | 10% | **NLP Tool:** Uses `language-tool-python`. Score = $1 - \min(\frac{\text{errors per 100 words}}{10}, 1)$. |
| **Vocabulary** | 10% | **Statistical:** Calculates Type-Token Ratio (TTR) = $\frac{\text{Unique Words}}{\text{Total Words}}$. |
| **Clarity** | 15% | **Pattern Matching:** Detects filler words (um, uh, like). Score drops as filler rate increases > 3%. |
| **Engagement** | 15% | **Sentiment Analysis:** Uses VADER to measure positivity probability. |

---

## 💻 Installation & Local Deployment
Follow these steps to run the application on your local machine.

### Prerequisites
- Python 3.8 or higher
- Java (Required for Grammar Checking library)

### Step 1: Clone the Repository
```bash
git clone [https://github.com/ASHISHMAHAJAN787/Nirmaan-ai-scorer.git](https://github.com/ASHISHMAHAJAN787/Nirmaan-ai-scorer.git)
cd nirmaan-ai-scorer

