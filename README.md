# ask-AI

Generate and run Bash commands using OpenAI’s GPT models.


![Demo](https://i.imgur.com/rqw3my6.gif)




## Requirements

* Bash
* curl
* OpenAI API key



## Install

```bash
curl -O https://raw.githubusercontent.com/zmsp/ask-bash/main/ask
chmod +x ask
mv ask ~/.local/bin/
export PATH="$PATH:$HOME/.local/bin"
ask --help
```



## Usage

```bash
ask "your task description"
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

