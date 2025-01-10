# Langchain Demo with OpenAI and LLaMA 2 APIs

This project demonstrates how to use the Langchain framework to create a simple Streamlit web app that integrates OpenAI's GPT-3.5 and Ollama's LLaMA 2 models. The app takes user input (a question) and generates a response based on the language model selected.

## Features

- **OpenAI GPT-3.5**: Using Langchain's integration with OpenAI's API.
- **LLaMA 2 (Ollama)**: Powered by the LLaMA 2 model via Ollama's API.
- **Streamlit Interface**: Provides a clean and interactive user interface to input questions and display answers.

## Setup

To run this project locally, follow the steps below:

### Prerequisites
- Python 3.7+
- Streamlit
- Langchain
- OpenAI API key
- Ollama API key (for LLaMA 2)
- `.env` file for storing sensitive keys

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/langchain-demo.git
   cd langchain-demo
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate # On Windows use venv\Scripts\activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the root directory with the following keys:
   ```plaintext
   OPENAI_API_KEY=<your_openai_api_key>
   LANGCHAIN_API_KEY=<your_langchain_api_key>
   ```

5. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## Usage

* Enter a question into the input field and click "Submit."
* The app will call either OpenAI's GPT-3.5 or LLaMA 2 (depending on the configuration) to generate an answer.
* You can select the model and interact with the assistant through the interface.

## Files in this Repository

1. `app.py` (OpenAI Demo): A Streamlit app using OpenAI's GPT-3.5 to answer user questions.
2. `app_llama.py` (LLaMA 2 Demo): A Streamlit app using LLaMA 2 (via Ollama API) to answer user questions.
3. `.env`: A configuration file to store your API keys securely.
4. `requirements.txt`: Lists the required Python packages for the project.

## Requirements (`requirements.txt`)
```txt
streamlit==1.14.0
langchain==0.0.147
openai==0.27.0
python-dotenv==0.21.0
llama-index==0.5.6
ollama==1.0.0
```

## License

This project is licensed under the MIT License - see the LICENSE file for details.
