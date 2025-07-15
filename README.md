---
title: Cot Llm 298
emoji: 💬
colorFrom: yellow
colorTo: purple
sdk: gradio
sdk_version: 5.23.3
app_file: app.py
pinned: false
license: cc-by-4.0
---

An chatbot using [Gradio](https://gradio.app), [`huggingface_hub`](https://huggingface.co/docs/huggingface_hub/v0.22.2/en/index), and the [Hugging Face Inference API](https://huggingface.co/docs/api-inference/index).

# Full-Stack LLM Tutoring App with Chain-of-Thought Reasoning

An interactive AI-powered learning assistant that combines secure authentication, a user-friendly Gradio interface, and the Hugging Face deployed models to simulate Chain-of-Thought (CoT) reasoning for deeper educational dialogue.

---

## Features

- **Full-Stack Functionality**: Includes user registration and login flow with in-memory credential management
- **LLM-Powered Tutor**: Integrates Mistral 7B model via Hugging Face API to generate step-by-step (CoT) explanations
- **Modular Design**: Clean separation of logic (helper functions) and UI (Gradio)
- **Gradio UI**: Tab-based interface for smooth interaction and theming
- **Chain-of-Thought Prompting**: Custom prompts guide the model to provide multi-step answers for better understanding

---

## Project Structure

├── app.py # Gradio frontend and session flow
├── helper_functions.py # API calls and CoT prompting logic
├── styles.css # Custom styles for Gradio components
├── .env # Hugging Face API key
├── requirements.txt # Python dependencies
└── README.md # Project overview and setup

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/anveshkumar0206/Full-Stack-LLM-Tutoring-App-with-CoT-Reasoning
cd Full-Stack-LLM-Tutoring-App-with-CoT-Reasoning

2. Install Dependencies
pip install -r requirements.txt

3. Configure Hugging Face Token
Create a .env file with:
HUGGINGFACEHUB_API_TOKEN=your_hf_token

Run the App python app.py
Open the Gradio URL shown in the terminal to use the app.

Sample Prompt
"Explain how to solve a quadratic equation using step-by-step reasoning."

The LLM will respond with a structured explanation using CoT prompting like:
Identify the coefficients a, b, and c.
Use the quadratic formula...
Calculate the discriminant...

Tech Stack

Frontend/UI: Gradio
Backend: Python, Hugging Face Inference AP
Model: mistralai/Mistral-7B-Instruct-v0.2
Authentication: Local user state management
CoT Prompting: Structured prompt engineering

Future Enhancements:

SQLite-based persistent login
Multi-turn chat memory
Subject-specific tutoring agents
Model selector dropdown
