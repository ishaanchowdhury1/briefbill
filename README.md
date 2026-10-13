# BriefBill

**Turn vague client briefs into clear freelance proposals — powered by Gemma 3.**

BriefBill is a local AI proposal assistant built for freelancers, independent developers, designers, and video editors. It helps turn informal client messages into structured project proposals while highlighting missing requirements and potential scope creep.

## Features

- **AI-powered brief analysis:** Uses Gemma 3 through Ollama to analyse client requirements.
- **Scope-risk detection:** Highlights ambiguous deliverables, missing details, and potential extra work.
- **Transparent pricing:** Calculates the base fee and contingency allowance using Python.
- **Editable proposals:** Review and refine the generated proposal before sharing it.
- **Export options:** Download the proposal and structured analysis.
- **Local inference:** When using Ollama locally, the brief is processed by the local model rather than a hosted AI API.

## Tech Stack

- Python
- Streamlit
- Ollama
- Gemma 3 (`gemma3:4b`)

## Run Locally

### 1. Install Ollama

Install Ollama from https://ollama.com/.

### 2. Download the model

```bash
ollama pull gemma3:4b
```

### 3. Clone this repository

```bash
git clone https://github.com/ishaanchowdhury1/briefbill.git
cd briefbill
```

### 4. Create a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 5. Install Python dependencies

```bash
pip install -r requirements.txt
```

### 6. Start BriefBill

Ensure Ollama is running, then execute:

```bash
streamlit run app.py
```

Open http://localhost:8501 in your browser.

## Important Notes

- AI-generated proposals may contain mistakes. Review all deliverables, assumptions, dates, and prices before sending them to a client.
- Pricing estimates are planning aids, not binding quotes.
- Unconfirmed scope items should be clarified with the client before work begins.
- This project currently runs locally and requires Ollama and a compatible downloaded model.

## Project Status

BriefBill is a working prototype. It is being tested with sample freelance briefs, and its scope-detection behaviour may need further improvement.
