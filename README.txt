# ChatGPT Command Translator

This script allows you to run commands translated from plain text descriptions using OpenAI's ChatGPT API. You can describe what you want to do in plain text, and the script will translate it into a command, which you can then choose to execute.

## Prerequisites

1. [Sign up](https://beta.openai.com/signup/) for an OpenAI API key.
2. Install `curl`, `jq`, and `zsh` on your system.

## Installation

1. Clone this repository:

``git clone https://github.com/yourusername/chatgpt-command-translator.git``


2. Change to the repository directory:

``cd chatgpt-command-translator``


3. Make the script executable:

``chmod +x chatgpt_cmd.zsh``

4. Set your OpenAI API key as an environment variable:

``export OPENAI_API_KEY="your_api_key_here"``

Optionally, you can add this line to your `.zshrc` or `.bashrc` file to set the API key automatically when you open a new terminal session. You will be prompted to enter your key if it isn't set.

## Usage

1. Run the script with a plain text description of what you want to do:

``./chatgpt_cmd.zsh "your_plain_text_description_here"``

For example:

./chatgpt_cmd.zsh "Create files named a.txt, b.txt,..., z.txt"


2. The script will display the translated command.

3. You will be prompted to choose whether you want to run the command, show the full API response, or exit without executing the command. To run the command, type `y` and press Enter. To show the full API response, type `d` and press Enter. To exit without executing the command, type `n` and press Enter.

## Notes

- The translated commands are executed using `eval`, so use this script with caution, as it may produce unexpected results or execute potentially harmful commands.
- Always review the translated commands before executing them to ensure they are safe and as expected.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
