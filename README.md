<a href="https://colab.research.google.com/github/officaldhanush/electronics-tutor-/blob/main/electronics-tutor.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>

# Electronics Tutor: AI explains, Python checks

A phone-friendly tutor for first-year electronics students, built in Google Colab with Python and Gradio.

## What it does
- **Ask tab:** answers electronics questions in simple English. A second AI call reviews each answer.
- **Quiz tab:** practice questions on Ohm's law, series and parallel resistors, and power.

## Key idea
Python creates each quiz question and works out the correct answer, so marking is always exact. The AI only explains: after a wrong answer, it gets the correct value and describes the likely mistake.

## How to run
1. Open the notebook in Google Colab.
2. Get a free API key from build.nvidia.com.
3. Run the cell, paste your key when asked, and choose an app password.
4. Open the public link shown. Never share it: anyone with it can use your key's allowance.

## Built with
Python, Gradio, the NVIDIA Build API with a Nemotron model, and the OpenAI Python SDK. Nothing in this repo runs on OpenAI's models.

## Limits
- The reviewer is the same model as the tutor, so it shares its blind spots.
- Only the number in a quiz answer is checked, not the unit.
- Currently runs on the NVIDIA Build API. Moving to Nebius Token Factory means changing the web address, the key, and the model name.

## What I learned
Prompts are part of the program. Use code where answers are exact, and AI where they are not.
