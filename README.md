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
    "[python]": {
        "editor.formatOnType": true // Formatar enquanto digita código Python
    },
    "files.exclude": {
        "**/.git": false // Incluir arquivos/diretórios .git no explorador
    },
    "security.allowedUNCHosts": [
        "wsl.localhost" // Permitir conexões UNCHost específicas, como para WSL
    ],
    "security.workspace.trust.untrustedFiles": "open", // Abrir arquivos não confiáveis
    "python.defaultInterpreterPath": "python", // Caminho padrão do interpretador Python
    "editor.formatOnSave": true, // Formatar automaticamente ao salvar
    "explorer.confirmDelete": false, // Desativar confirmação ao excluir arquivos
    "terminal.integrated.defaultLocation": "editor", // Abrir terminal integrado na área do editor
    "diffEditor.ignoreTrimWhitespace": false, // Considerar espaços em branco ao comparar diferenças
    "files.trimTrailingWhitespace": true, // Remover espaços em branco no final das linhas ao salvar
    "editor.cursorSmoothCaretAnimation": "on", // Ativar animação suave do cursor
    "editor.cursorBlinking": "expand", // Definir piscamento do cursor como expandido
    "workbench.iconTheme": "material-icon-theme", // Tema de ícones do Workbench
    "workbench.colorTheme": "Min Dark", // Tema de cores do Workbench
    "editor.fontSize": 14, // Tamanho da fonte do editor
    "editor.fontFamily": "JetBrains Mono, 'Courier New', monospace", // Família de fontes do editor
    "editor.lineHeight": 1.8, // Altura da linha do editor
    "workbench.startupEditor": "newUntitledFile", // Abrir novo arquivo em branco ao iniciar
    "editor.renderLineHighlight": "gutter", // Destacar linha atual na margem esquerda
    "editor.fontLigatures": true, // Ativar ligaduras de fonte no editor
    "workbench.editor.labelFormat": "short", // Mostrar nomes curtos para abas de editores
    "explorer.compactFolders": false, // Desativar exibição compacta de pastas
    "editor.semanticHighlighting.enabled": false, // Desativar realce semântico no editor
    "breadcrumbs.enabled": false, // Desativar breadcrumbs (caminho de navegação)
    "editor.minimap.enabled": false, // Desativar minimapa no editor
    "window.commandCenter": false, // Desativar command center na janela do VS Code
    "window.menuBarVisibility": "compact", // Visibilidade da barra de menu
    "workbench.layoutControl.enabled": false, // Desativar controle de layout do workbench
    "terminal.integrated.defaultProfile.windows": "Git Bash", // Perfil padrão do terminal integrado
    "files.autoSave": "onFocusChange" // Salvar automaticamente ao mudar de foco
}
