# VSCode Keybindings

In the online IDE, pasting into the terminal with CTRL+V / CMD+V doesn't work because there's a keybinding that intercepts the command and prevents the pasting action.

The `keybindings.json` that's meant to be used to edit keybindings only gets created at runtime after the _user_ initializes a keybinding change. Since we can't ask users to modify this keybinding manually every session, and MSFT [doesn't want to support workspace level keybindings](https://github.com/Microsoft/vscode/issues/4504), we have to create a custom extension that does this, similar to [this](https://github.com/Microsoft/vscode-sublime-keybindings).
