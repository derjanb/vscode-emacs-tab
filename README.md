# vscode-emacs-tab

![screencast](emacs-tab.gif)

This plugin provides `emacs-tab.reindentCurrentLine`
command, which indents like emacs behavior.

1. Always indent a line to the same level
2. Move the cursor to the first character if cursor is in
the leading white spaces.

In order to change 'tab' key behavior, please write the following lines
in your `keybindings.json`.

```json
{
  "key": "tab",
  "command": "emacs-tab.reindentCurrentLine",
  "when": "editorTextFocus"
}
```
## Installation

```bash
npm install -g vsce

git clone https://github.com/derjanb/vscode-emacs-tab.git
cd vscode-emacs-tab
npm install
vsce package
code --install-extension vscode-emacs-tab-0.0.9.vsix
```
