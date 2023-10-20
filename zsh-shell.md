# Overview

This is my personal setup for linux (Ubuntu) to install `oh-my-zsh` shell and setup with `powerlever10k` theme

# Instructions

1. Install `zsh`

   ```console
   sudo apt install zsh
   ```

2. Install `oh-my-zsh`

   ```console
   sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```

3. Close session and restart (this will make zsh shell default)

4. Copy the content of `.zshrc` file into your system file

5. Install `powerlever10k` Fonts

   - [MesloLGS NF Regular.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf)
   - [MesloLGS NF Bold.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf)
   - [MesloLGS NF Italic.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf)
   - [MesloLGS NF Bold Italic.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf)

6. Change font in terminal

## Zsh plugins

### Zsh-autosuggestions

1. Run the command

   ```console
   git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
   ```

2. Uncomment the plugin in file

## FNM

1. Run command

   ```console
   curl -fsSL https://fnm.vercel.app/install | bash
   ```

2. Uncomment Fnm section

## Golang

1. Install golang from official webpage

2. Uncomment Go section

## Functions

often I likie to create zsh functions to automate a little bit of my life, here an example

```console
gcommit() {
  if [ n != "" ]
  then
    git add .
    git commit -m "$1"
    git push
  else
    echo "YOU MUST PROVIDE A MESSAGE"
  fi
}
```
