# Oh My Zsh

## Install with curl

```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Enabling Plugins

### Download Plugins

```sh
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
git clone https://github.com/marlonrichert/zsh-autocomplete.git $ZSH_CUSTOM/plugins/zsh-autocomplete
```

### Configure ~/.zshrc

Open the config file:

```sh
nano ~/.zshrc
```

Find `plugins=(git)` and update it to:

```sh
plugins=(git zsh-autosuggestions zsh-syntax-highlighting zsh-autocomplete)
```

Reopen your terminal or run `source ~/.zshrc` to apply changes.

### What Each Plugin Does

- **zsh-autosuggestions** — suggests commands as you type based on your history
- **zsh-syntax-highlighting** — highlights valid commands in green and invalid ones in red
- **zsh-autocomplete** — adds real-time tab completion with a live dropdown menu
