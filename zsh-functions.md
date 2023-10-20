# Introduction

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
