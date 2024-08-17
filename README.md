# AI-Powered CLI 

This project leverages the power of Google's Gemini large language model to create an intuitive command-line interface (CLI) that understands natural language input and translates it into executable terminal commands.

## Features

* **Natural Language Understanding:**  Users can interact with the CLI using everyday language to express their intent.
* **Command Translation:** The Gemini model interprets user input and generates the corresponding terminal command.
* **User Confirmation:** Before executing any command, the CLI seeks confirmation from the user to ensure safety and prevent unintended actions.
* **Error Handling:**  Robust error handling mechanisms are in place to gracefully deal with invalid commands or unexpected situations.

## Installation

1. **Clone the Repository:**
   ```bash
   git clone [invalid URL removed]
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Gemini API Key:**
   * Obtain a Gemini API key from Google.
   * Set the `GEMINI_API_KEY` environment variable:

    ```bash
    export GEMINI_API_KEY='YOUR_ACTUAL_API_KEY' 
    ```

## Usage

1. **Run the CLI:**
   ```bash
   python3 main.py
   ```

2. **Interact with the CLI:**
   * The CLI will prompt you with `$ask `. 
   * Type your request in natural language (e.g., "Show me all the files in this directory").
   * The CLI will suggest a terminal command.
   * Confirm the execution by typing `y` and pressing Enter.

## Example

```
$ask list all files in this directory
> Execute "ls -l"? [y/N] y
# Output of the `ls -l` command will be displayed here
```

## Important Notes

* **Security:** Exercise caution when executing commands generated by the AI. Always review the suggested command before confirming its execution.
* **Model Limitations:** The accuracy of command translation depends on the capabilities of the Gemini model.  There might be instances where the model misunderstands the intent or generates incorrect commands.
* **Error Reporting:**  If you encounter any errors or unexpected behavior, please report them on the project's issue tracker.

## Contributing

Contributions are welcome!  Please read the CONTRIBUTING.md file for guidelines on how to contribute to this project.

## License

This project is licensed under the MIT License.  See the LICENSE file for details.