# Local LLM CLI

## Overview

The AI Query Engine is a modernized script designed to interact with AI models through either LM Studio or OpenRouter. It provides a user-friendly interface for sending prompts and displaying responses in an elegant, colorful format.

## Features

- **Backend Support**: Connects to either LM Studio or OpenRouter for AI responses.
- **Prompt Handling**: Accepts input from the terminal, piped input, or command-line arguments.
- **Modern Output**: Uses ANSI color codes and formatting tools like `bat` or `glow` for beautiful terminal output.
- **Loading Spinner**: Provides a visual indicator while waiting for AI responses.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/local-llm-cli.git
   cd local-llm-cli
   ```


2. Install dependencies:
   sudo apt-get install jq bat glow  # For Debian-based systems
   

## Configuration

Edit the `config.sh` file to set your API keys and other configurations:

```
BACKEND="lmstudio"  # Options: "lmstudio" or "openrouter"
LM_HOST="192.168.0.103"
LM_PORT="1234"
OPENROUTER_API_KEY="your_openrouter_api_key_here"
OPENROUTER_MODEL="z-ai/glm-4.5-air:free"
```

## Usage

### From Terminal

```bash
./query.sh "Your prompt here"
```

### Piped Input

```bash
echo "Your prompt here" | ./query.sh
```

### Interactive Mode

```bash
./query.sh
```


## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

GNU General Public License v3.0
