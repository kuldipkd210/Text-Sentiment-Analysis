# Text-Sentiment-Analysis
A web application built with Flask and TextBlob to analyze text sentiment (Positive, Negative, Neutral) with polarity and subjectivity scores.

Flask Sentiment Analysis Web App


#Tech Stack

Python 3.x

Flask

TextBlob

HTML5

CSS3


A simple and clean Sentiment Analysis web application built using:

Flask (Backend Web Framework)

TextBlob (Natural Language Processing)

HTML + CSS (Frontend UI)

This application analyzes user input text and classifies it as:

Positive

Negative

Neutral

It also displays:

Polarity score

Subjectivity score

1. Project Overview

This project demonstrates:

Handling HTTP GET and POST requests in Flask

Using TextBlob for NLP-based sentiment analysis

Rendering dynamic results using Jinja2 templates

Displaying calculated metrics on a web interface

It is ideal for:

Beginners learning Flask

Students exploring NLP basics

Portfolio projects

2. How Sentiment Analysis Works

TextBlob provides two important values:

Polarity

Range: -1 to +1

-1 → Very Negative

+1 → Very Positive

Subjectivity

Range: 0 to 1

0 → Objective (fact-based)

1 → Subjective (opinion-based)

Classification Logic Used
if polarity > 0.1:
    sentiment = "Positive"
elif polarity < -0.1:
    sentiment = "Negative"
else:
    sentiment = "Neutral"

3. Project Structure
sentiment-analysis-app/
│
├── app.py
├── templates/
│   └── index.html
├── static/
│   └── style.css
└── README.md

4. Installation Guide (Step-by-Step)
Step 1: Clone the Repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name


Or download the ZIP file and extract it.

Step 2: Create Virtual Environment (Recommended)
python -m venv venv


Activate it:

Windows

venv\Scripts\activate


Mac/Linux

source venv/bin/activate

Step 3: Install Required Libraries
pip install flask textblob


After installing TextBlob, run:

python -m textblob.download_corpora


This downloads required NLP datasets.

5. Running the Application

Run the following command:

python app.py


You will see output like:

Running on http://127.0.0.1:5000/


Open your browser and go to:

http://127.0.0.1:5000/

6. How to Use the App

Enter any sentence or paragraph in the text box.

Click Analyze Text.

View:

Sentiment classification

Polarity score

Subjectivity score
