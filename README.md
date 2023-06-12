# cli-tools

This repository is a collection of versatile bash scripts aimed to simplify various tasks on a macOS environment. They can be placed anywhere within your PATH for easy access.

## Scripts

### `rpass`

Generates a secure, random password and copies it to the clipboard. It uses pwgen for generating the password and pbcopy (macOS) for clipboard operations. The script checks for pwgen and attempts to install it if not present.

> Usage: `rpass`

**Dependencies**: `pwgen` (The script checks for `pwgen` and gives install instructions if not present.)

### `rname`

Generates two random proper names using the list of proper names available on Unix-based systems and copies them to the clipboard.

> Usage: `rname`

### `gpterm`

A bash interface for OpenAI's GPT models. It takes the model name and a system message as input and interacts with the model using OpenAI's API.


```shell
# Usage:
gpterm -m MODEL -s SYSTEM_MESSAGE USER_MESSAGE [USER_MESSAGE...]
```

**Dependencies:** `jq` (The script checks for `jq` and attempts to install it if not present.)

### `looksee`

Fetches a webpage, converts it to text, tokenizes it, and feeds the tokens into a long-lived model. It takes a URL and a system name as input.

```shell
# Usage: 
looksee URL SYSTEM
```

**Dependencies:** `html2text`, `ttok`, `llm` (Please ensure these are installed and in your PATH.)

## Contributions

Feel free to clone, use, or tweak these scripts as needed. Your contributions to improve these scripts or add new ones are welcome!