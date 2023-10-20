# Snippets

Click on engine in the lower left corner and then in `configure user snipets`

1. write `Javascript` and hit enter, a example code will look like this

   ```javascript
   {
    "Print to console": {
      "prefix": "log",
      "body": [
        "console.log('$1');",
        "$2"
      ],
      "description": "Log output to console"
    }
   }
   ```

   The `$1` is the tabs movements

# Plugins

1. [material icon](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
2. [Auto close tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag)
3. [Auto rename tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
4. [auto complete tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-complete-tag)
5. [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
6. [Eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
7. [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
8. [JS ES6 snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets)
9. [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
10. [Turbo console log](https://marketplace.visualstudio.com/items?itemName=ChakrounAnas.turbo-console-log)

# Personal configuration

This is my personal taste in vscode folded in `settings.json`

1. `ctrl+,` to open settings
2. search `editor ui`
3. in `Workbench › Settings: Editor` select `json`
4. save

```json
{
  "workbench.iconTheme": "material-icon-theme",
  "editor.fontSize": 18,
  "editor.formatOnSave": true,
  "editor.tabSize": 2,
  "editor.renderWhitespace": "all",
  "go.toolsManagement.autoUpdate": true,
  "editor.fontLigatures": true,
  "editor.fontFamily": "'Cascadia Code', Menlo, Monaco, 'Courier New', monospace",
  "terminal.integrated.fontFamily": "MesloLGS NF",
  "terminal.integrated.fontSize": 14,
  "workbench.editor.languageDetection": true,
  "gitlens.hovers.currentLine.over": "line",
  "telemetry.telemetryLevel": "off",
  "[javascript]": {
    "editor.maxTokenizationLineLength": 2500,
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[css]": {
    "editor.suggest.insertMode": "replace",
    "gitlens.codeLens.scopes": ["document"],
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[graphql]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "protoc": {
    "options": [
      "--proto_path=proto",
      "--proto_path=${workspaceRoot}/proto",
      "--proto_path=${env.GOPATH}/src",
      "--java_out=gen/java"
    ]
  },
  "git.confirmSync": false,
  "git.autofetch": true,
  "security.workspace.trust.untrustedFiles": "open",
  "javascript.updateImportsOnFileMove.enabled": "always",
  "terminal.explorerKind": "external",
  "workbench.settings.editor": "json",
  "vs-kubernetes": {
    "vscode-kubernetes.helm-path.linux": "/home/kiyoshi/.local/state/vs-kubernetes/tools/helm/linux-amd64/helm"
  },
  "extensions.ignoreRecommendations": true,
  "[yaml]": {
    "editor.defaultFormatter": "redhat.vscode-yaml"
  },
  "cmake.configureOnOpen": true,
  "liveServer.settings.donotShowInfoMsg": true
}
```

## Extras

1. [install cascadia code font](https://www.youtube.com/watch?v=PaAT5n4fEcY&t=207s)
2. [install cascadia code vscode](https://www.youtube.com/watch?v=_r511M0Yzq0)
