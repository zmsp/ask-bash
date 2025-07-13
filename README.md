# ask-AI — Bash Script Powered by OpenAI

A simple CLI tool that helps you generate and run Bash commands using OpenAI's GPT models.

![Demo](https://i.imgur.com/rqw3my6.gif)

---

## Features

* Quickly get a Bash command for any task description
* Uses OpenAI’s Chat API (`gpt-4.1-nano`)
* Minimal dependencies — just Bash, `curl`
* Automatically saves your API key securely
* Optional interactive execution mode

---

## Requirements

* Bash
* [`curl`](https://curl.se/)
* [`jq`](https://stedolan.github.io/jq/)
* OpenAI API key (get one at [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys))

---

## Installation

1. Download the script:

   ```bash
   curl -O https://raw.githubusercontent.com/zmsp/ask-bash/main/ask
   ```

2. Make it executable:

   ```bash
   chmod +x ask
   ```

3. Move it into your PATH (optional but recommended):

   ```bash
   mv ask ~/.local/bin/
   export PATH="$PATH:$HOME/.local/bin"
   ```

4. Set your OpenAI API key (once):
   You can either:

   * Export it in your terminal:

     ```bash
     export OPENAI_API_KEY="sk-REPLACE_ME"
     ```
   * Or run the script once and it will prompt you to paste the key and save it to `~/.openai_api_key` securely.

---

## Usage

```bash
ask "list all .log files in /var and delete them"
```

Sample output:

```
Suggested command:
find /var -name '*.log' -delete

Run this command? (y/n): n
Cancelled.
```

### Options

```bash
ask --help
```

### Environment Variables

| Variable         | Purpose                                      |
| ---------------- | -------------------------------------------- |
| `OPENAI_API_KEY` | Your OpenAI API key. Required.               |
| `VERBOSE=true`   | Optional. Enables debug output and raw JSON. |

---

## Examples

```bash
ask "untar a .tar.gz file"
ask "find files over 100MB in /home"
ask "restart nginx only if it's not running"
```

---

## Contributing

Contributions welcome.
If you find a bug or want to suggest an improvement, please open an issue or submit a pull request.

---

## License

MIT License © Zobair

---

Let me know if you want it even more minimal or focused on usage tips.
