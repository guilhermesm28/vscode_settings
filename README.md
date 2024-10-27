# Minhas configurações no VS Code

Este repositório contém minhas configurações personalizadas para o VS Code. Aqui você encontrará as extensões e configurações que uso para otimizar meu fluxo de trabalho.

## Extensões

Lista de extensões que utilizo:

- **CodeSnap**: adpyke.codesnap
- **Docker**: ms-azuretools.vscode-docker
- **iSort**: ms-python.isort
- **Jupyter**: ms-toolsai.jupyter
- **Jupyter Cell Tags**: ms-toolsai.vscode-jupyter-cell-tags
- **Jupyter Keymap**: ms-toolsai.jupyter-keymap
- **Jupyter Notebook Renderers**: ms-toolsai.jupyter-renderers
- **Jupyter Slide Show**: ms-toolsai.vscode-jupyter-slideshow
- **Material Icon Theme**: PKief.material-icon-theme
- **Min Theme**: miguelsolorio.min-theme
- **Pylance**: ms-python.vscode-pylance
- **Python**: ms-python.python
- **Python Debugger**: ms-python.debugpy
- **Rainbow CSV**: mechatroner.rainbow-csv
- **WSL**: ms-vscode-remote.remote-wsl

## Configurações

### Font Family

O primeiro passo antes de copiar o arquivo de configurações JSON é instalar a fonte [JetBrains Mono](https://www.jetbrains.com/lp/mono/)

### Settings.json

Estas são as configurações que uso no meu `settings.json`:

```json
{
    "security.workspace.trust.untrustedFiles": "open",
    "python.defaultInterpreterPath": "python",
    "editor.formatOnSave": true,
    "[python]": {
        "editor.formatOnType": true
    },
    "explorer.confirmDelete": false,
    "files.defaultLanguage": "r",
    "terminal.integrated.defaultLocation": "editor",
    "diffEditor.ignoreTrimWhitespace": false,
    "files.trimTrailingWhitespace": true,
    "editor.cursorSmoothCaretAnimation": "on",
    "editor.cursorBlinking": "expand",
    "security.allowedUNCHosts": [
        "wsl.localhost"
    ],
    "workbench.iconTheme": "material-icon-theme",
    "files.exclude": {
        "**/.git": false
    },
    "workbench.colorTheme": "Min Dark",
    "editor.fontSize": 14,
    "editor.fontFamily": "JetBrains Mono, 'Courier New', monospace",
    "editor.lineHeight": 1.8,
    "workbench.startupEditor": "newUntitledFile",
    "editor.renderLineHighlight": "gutter",
    "editor.fontLigatures": true,
    "workbench.editor.labelFormat": "short",
    "explorer.compactFolders": false,
    "editor.semanticHighlighting.enabled": false,
    "breadcrumbs.enabled": false,
    "editor.minimap.enabled": false,
    "window.commandCenter": false,
    "window.menuBarVisibility": "compact",
    "workbench.layoutControl.enabled": false,
    "terminal.integrated.defaultProfile.windows": "Git Bash",
    "files.autoSave": "onFocusChange"
}
