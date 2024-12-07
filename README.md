# Chat CLI Assistant

A command-line assistant powered by a Language Model API (LLM), allowing you to interact with an AI directly from your terminal.

## Features

- Send requests to a LLM API to get intelligent responses.
- Interactive command-line interface to send custom messages.
- Displays model-generated responses directly in the terminal.

## TODO 
- make env variable for API_KEY and the model
- choose which model you want
- add more context
- choose the parameters such as temp and tokens numbers 

## Prerequisites

- Python 3.x
- A valid API key for the Groq API (or another compatible LLM provider).

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/dre4ft/chat_cli.git
   cd chat_cli
   ```
2. Install dependencies:
   ```bash
   pip install Groq
   ```
3. Add your API key in the code:
   ```python
   GROQ_API_KEY = "your-api-key"
   ```
3. change the shebang if needed:
   ```python
   #!/usr/bin/env python3
   ```
3. change the base prompt to fit your use case :
   ```python
   base_prompt = """your an assistant specialized in coding in C++"""
   ```

## Usage

1. Run the script in your terminal:
   ```bash
   ./chat_cli
   ```

2. Enter your message when prompted.

3. The AI assistant will respond directly in the terminal.

### Example

```bash
Enter your message: Who is the president of the United States?
Assistant's Response:
The president of the United States is Joe Biden.
```

## Make it globally accessible

You can place the script in a directory like `~/bin` and add this directory to your `$PATH` to make the command accessible from anywhere on your machine.

1. Move the script to `~/bin` (or another directory):
   ```bash
   mv chat_cli ~/.bin/chat_cli
   ```
   
2. change the permissions for exemple :
   ```bash
   chmod 700 chat_cli
   ```  

3. Make sure `~/bin` is in your `$PATH`. To do this, edit your shell's configuration file (e.g., `~/.bashrc` or `~/.zshrc`) and add:
   ```bash
   export PATH="$HOME/.bin:$PATH"
   ```

4. Reload your shell configuration:
   ```bash
   source ~/.bashrc   # or source ~/.zshrc
   ```

5. Now, you can run the assistant from anywhere in your terminal by typing:
   ```bash
   chat_cli
   ```

## Troubleshooting

- If you encounter any issues during installation or execution, please open an issue on this repository.

---

This README includes the setup, usage, and the steps to make your script globally accessible by adding it to your `$PATH`. Feel free to modify the content according to your project's details or any future updates!
