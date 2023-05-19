# ask-AI Bash Script

Simple bash script that helps you with bash commands using the Power of AI

![Alt Text](https://i.imgur.com/rqw3my6.gif)

## Features

- Generates Bash commands tailored to your specific task
- Makes use of the OpenAI API for intelligent command generation
- Easy to use and execute with simple command-line interface

## Requirements
* Bash terminal
* Open AI api key from  https://platform.openai.com/account/api-keys

## Installation

1. Download the Awesome Bash Script using curl:
   ```bash
   $ curl -O https://raw.githubusercontent.com/zmsp/ask-bash/main/ask
   ```


2. Make the script executable:
   ```bash
   $ chmod +x ask
   ```

3. Update some environmental variables:
   ```bash
    export PATH="$PATH:/path/to/ask"
    export VERBOSE="false"       Disable verbose mode
    export OPEN_AI_KEY="REPLACE_ME_XXXX"     Specify your OPEN-AI key from https://platform.openai.com/account/api-keys
   ```
4. Profit
   ```bash
    ask --help
    ask delete all files recursively on root directory
    Verbose turned on
    Command:
    rm -rf /*
    Run the command? (y/n): n
    Nope...
   ```

## Usage
For more information and available options, refer to the built-in help:

```bash
ask help
$ ask untar a directory
```


## Contributing

Welcome contributions! If you find a bug or have a suggestion, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. 

---

Happy scripting!