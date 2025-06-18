# ai_text_completion_project

# 🧠 Hugging Face Text Completion App (Console Version)

This is a simple, interactive Python application that uses Hugging Face’s **Inference API** to generate text completions using the `HuggingFaceH4/zephyr-7b-beta` model. It is designed to run in **Google Colab** or any Python environment with console input support.

## 🚀 Features

- Input prompts interactively through the console.
- Choose generation parameters: `temperature`, `top_p`, and `max_new_tokens`.
- Input validation for safe interaction.
- Handles API errors, timeouts, and invalid input.
- Easy to customize or extend for other models or tasks.
- 
## Setup

Step 1
Python: You could use Google colab or vscode for run the app
Paste and run the full script provided 

Step 2
You’ll be prompted to input your Hugging Face token securely.
Configurate Hugging Face Access Token
You need a Hugging Face access token to use the Inference API.
Go to https://huggingface.co/settings/tokens and create a new token with the "read" role.

Step 3 
You will be asked to:
- Enter your prompt (e.g. “Write a poem about the sea”)
- Choose `temperature` (creativity level)
- Choose `max_new_tokens` (response length)
- Choose `top_p` (sampling diversity)

Type `quit`, `exit`, or `stop` to end the session.

## ❗ Common Errors and Solutions

- **401 Unauthorized**: Invalid API token. Re-check token or permissions.
- **422 Error**: Model may not support raw `text-generation` — ensure you’re using a compatible model.
- **Timeout**: Network issues or slow model. Try again or increase timeout.
- **Empty Prompt**: The app checks for this and returns an error.
