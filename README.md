# AI MCQ Quiz Generator

## Project Overview

AI MCQ Quiz Generator is a Streamlit-based web application that uses Hugging Face AI to generate multiple-choice questions automatically based on a topic entered by the user.

The application allows users to:

* Enter any topic
* Select the number of questions
* Generate MCQ questions using AI
* Select answers for each question
* Submit the quiz
* View the final score

The project was developed using Visual Studio Code.

## Technologies Used

* Python
* Streamlit
* Hugging Face Inference API
* Hugging Face Hub
* JSON
* OpenAI GPT-OSS-120B model through Hugging Face

## Project Structure

```text
mcq_quiz_app/
│
├── app.py
├── requirements.txt
├── README.md
└── .streamlit/
    └── secrets.toml
```

## Features

### 1. Topic Input

Users can enter a topic for the quiz, such as:

```text
Python
```

### 2. Question Count

Users can select between 1 and 10 questions.

### 3. AI-Based Question Generation

The application sends the selected topic and question count to the Hugging Face AI model and generates multiple-choice questions.

### 4. Multiple Choice Questions

Each generated question contains four answer options.

### 5. Quiz Submission

Users can select an answer for each question and submit the quiz.

### 6. Score Calculation

The application compares the selected answers with the correct answers and displays the final score.

## Requirements

Install the required Python packages using:

```bash
pip install -r requirements.txt
```

The `requirements.txt` file should contain:

```text
streamlit
huggingface_hub
```

## Hugging Face API Token Setup

This project requires a Hugging Face API token.

Create the following folder inside the project:

```text
.streamlit
```

Inside the `.streamlit` folder, create:

```text
secrets.toml
```

Add your Hugging Face token:

```toml
HF_TOKEN = "your_huggingface_token"
```

Replace `your_huggingface_token` with your actual Hugging Face API token.

Do not share your API token publicly.

## How to Run the Project

### Step 1: Open the Project in VS Code

Open the `mcq_quiz_app` folder in Visual Studio Code.

### Step 2: Open the Terminal

In VS Code, select:

```text
Terminal → New Terminal
```

### Step 3: Install Requirements

Run:

```bash
python -m pip install -r requirements.txt
```

### Step 4: Run the Streamlit Application

Run:

```bash
python -m streamlit run app.py
```

The application will open in the web browser.

## How to Use

1. Enter a topic in the topic input box.
2. Select the number of questions.
3. Click the `Generate Quiz` button.
4. Wait for the AI to generate the questions.
5. Select an answer for each question.
6. Click the `Submit Quiz` button.
7. The application displays your score.

## Example

Input:

```text
Topic: Python
Number of questions: 5
```

The AI generates five Python-related multiple-choice questions.

After answering all questions, the application displays a result such as:

```text
Your score: 4/5
```

## AI Model

The project uses the following Hugging Face model:

```text
openai/gpt-oss-120b
```

The model is accessed through the Hugging Face `InferenceClient`.

## Python Concepts Used

This project demonstrates several Python concepts:

* Variables
* Conditional statements
* Lists
* Dictionaries
* Loops
* Functions and API calls
* Exception handling
* JSON parsing
* Streamlit session state

## Future Enhancements

The application can be improved by adding:

* Timer for the quiz
* Difficulty selection
* Negative marking
* Question explanations
* Quiz history
* Percentage calculation
* Restart quiz option
* Downloadable quiz results
* Different question categories

## Author

Keerthana

