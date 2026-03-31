# 🎯 Student Stress Detector

A Python-based command-line tool designed to help students track their emotional well-being using Natural Language Processing (NLP). This application analyzes daily reflections to identify stress levels and provides a weekly overview of your mood.

---

## 📋 Features

* **Daily Mood Logging**: Record how you're feeling with a text entry.
* **Sentiment Analysis**: Automatically calculates a sentiment score (compound) to determine if you are "Stressed," "Neutral," or "Positive".
* **Historical Tracking**: View previous entries with their dates and scores.
* **Weekly Summary**: Generates an overall mood report based on all your logged entries.

---

## ⚙️ Setup & Installation

To run this project on your local machine, follow these steps:

### 1. Prerequisites
Ensure you have **Python 3.x** installed on your system.

### 2. Install Dependencies
This project uses the `nltk` library for sentiment analysis. Install it via terminal/command prompt:
```bash
pip install nltk
```

### 3. Download the Lexicon
The analyzer requires the VADER lexicon to function. You can download it by running this one-liner in your terminal:
```bash
python -c "import nltk; nltk.download('vader_lexicon')"
```

---

## 🚀 How to Use

1.  Navigate to the project directory.
2.  Run the application:
    ```bash
    python main.py
    ```
3.  **Menu Options**:
    * **1**: Log a new entry about your day.
    * **2**: View all your saved entries.
    * **3**: Generate a weekly summary and see your average sentiment.
    * **0**: Exit the program.

---

## 📂 Project Structure

* **`main.py`**: The main entry point and user interface logic.
* **`analyzer.py`**: Handles text processing and sentiment scoring using VADER.
* **`storage.py`**: Manages the saving and loading of data to `entries.json`.
* **`entries.json`**: (Auto-generated) Stores your personal logs locally.

---
