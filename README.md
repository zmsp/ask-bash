# ask-AI

Generate and run Bash commands using OpenAI’s GPT models.


![Demo](https://i.imgur.com/rqw3my6.gif)




## Requirements

* Bash (any linux based system)
* [curl](https://everything.curl.dev/install/)
* [jq](https://jqlang.org/download/)
* [OpenAI API key](https://platform.openai.com/settings/organization/api-keys)



## Install

```bash
curl -fsSL https://raw.githubusercontent.com/zmsp/ask-bash/main/ask -o /tmp/ask
chmod +x /tmp/ask
sudo mv /tmp/ask /usr/local/bin/
ask --help
```



## Usage
Generate a bash command for a task and optionally run it:
```bash
ask your task description
```

Send a direct question or prompt to the API (skips “run this command” behavior with `-` flag):
```bash
ask -q Explain the ls command options
```
Set your API key by exporting `OPENAI_API_KEY` or let the script prompt and save it.


## Options

```bash
ask --help
```


## Env Variables

* `OPENAI_API_KEY` — your OpenAI key (required). You can either:

  * Export it in your current shell:

    ```bash
    export OPENAI_API_KEY="your_api_key_here"
    ```
  * Or run the script once and it will prompt you to paste the key and save it securely to `~/.openai_api_key`.

* `VERBOSE=true` — enable debug output (optional)

## License

MIT © Zobair

