[
  {
    "keys": ["ctrl+w"],
    "command": "chain",
    "args": {
      "commands": [
        ["insert_snippet", { "contents": "|" }]
      ]
    }
  },
  {
    // Create puts for debugger purposes
    "keys": ["ctrl+p"],
    "command": "chain",
    "args": {
      "commands": [
        ["insert", { "characters": "puts " }],
        ["insert_snippet", { "contents": "'$0'" }],
        ["insert", { "characters": "#" }],
        ["move", { "by": "characters", "forward": true }],
        ["insert", { "characters": "*80" }],
        ["insert", { "characters": "\n" }],
        ["insert", { "characters": "puts" }],
        ["insert", { "characters": " " }],
        ["insert_snippet", { "contents": "'$0'" }],
        ["insert", { "characters": "#" }],
        ["move", { "by": "characters", "forward": true }],
        ["insert", { "characters": "*80" }],
        ["move", { "by": "lines", "forward": false }],
        ["insert", { "characters": "\nputs ''" }],
        ["move", { "by": "characters", "forward": false }]
      ]
    }
  },
  {
    // Transform {...} into do...end blocks.
    // Place the cursor here(*) => a.map { |e| *e + 2 }
    "keys": ["ctrl+b"],
    "command": "chain",
    "args": {
      "commands": [
        ["insert", { "characters": "\n" }],
        ["expand_selection", { "to": "brackets" }],
        ["copy"],
        ["left_delete"],
        ["run_macro_file", { "file": "res://Packages/Default/Delete Left Right.sublime-macro" }],
        ["insert", { "characters": "do end" }],
        ["move", { "by": "characters", "forward": false }],
        ["move", { "by": "characters", "forward": false }],
        ["move", { "by": "characters", "forward": false }],
        ["move", { "by": "characters", "forward": false }],
        ["move", { "by": "characters", "forward": true }],
        ["insert", { "characters": "\n\n" }],
        ["move", { "by": "lines", "forward": false }],
        ["left_delete"],
        ["left_delete"],
        ["paste"],
      ]
    }
  }
]
