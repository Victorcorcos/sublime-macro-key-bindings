# sublime-macro-key-bindings

Dedicated to share sublime macro key bindings for *Ruby* language.

Sublime can create macros natively (with Ctrl+q), but you cannot associate them with keybindings by default!

#### Why?
Because Sublime keybindings can only be associated with one command *natively*, not a list of commands. To enable this feature, it is necessary to install the **ChainOfCommand** plugin, which allows you to associate keybindings to list of commands.

### Example:
```json
{
  "keys": ["super+shift+option+d"], 
  "command": "chain", 
  "args": {
    "commands": [
      ["select_all"],
      ["copy"],
      ["new_file"],
      ["paste"],
      ["save"]
    ]
  }
}
```

I'll share some macro keybindings here that I created using macros and transferring the result to a keybinding using **ChainOfCommand**.

The keybindings should be added in "*Sublime Text* > *Preferences* > *Key Bindings*" file
