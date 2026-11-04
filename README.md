# LAB5 Calculator Web App

A small Flask web application that performs basic arithmetic operations on two numbers and displays the results in the browser.

## Features

- Addition
- Subtraction
- Multiplication
- Division
- Safe handling for division by zero

## Project structure

- `app.py` — Flask application and calculator logic
- `integration_test.py` — basic integration test for the calculator
- `Dockerfile` — container setup for running the app

## Requirements

- Python 3.9+
- Flask

## Run locally

1. Create and activate a virtual environment (optional but recommended):
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```
2. Install dependencies:
   ```bash
   pip install Flask
   ```
3. Start the app:
   ```bash
   python app.py
   ```
4. Open the app in your browser at:
   ```text
   http://localhost:5000
   ```

## Run with Docker

```bash
docker build -t lab5-calculator .
docker run -p 5000:5000 lab5-calculator
```

Then visit:
```text
http://localhost:5000
```

## Testing

Run the integration test with:

```bash
python -m unittest integration_test.py
```
