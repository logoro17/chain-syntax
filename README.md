# Chain-Lang VSCode Extension (`Chain-lang`)

Official VSCode syntax highlighting and language support extension for **Chain-Lang**, the custom programming language powering the **NebulaOS** ecosystem.

## Features

- **Advanced Syntax Highlighting**: Accurate colorization for control flow keywords, storage types, built-in functions, constants, numbers (including hex literals), and strings.
- **Smart Operator Precedence**: Clean and error-free operator matching (`==`, `!=`, `<=`, `>=`, `+`, `-`, `*`, `/`, `=`, `<`, `>`, `and`, `or`).
- **C++ Interoperability Support**: Embedded `extern "c"` C++ block scope highlighting (`source.cpp`).
- **Function Call Highlighting**: Automatically detects and highlights user-defined or built-in function calls.
- **Editor Configuration**:
  - Line comment support using `#`.
  - Automatic bracket and quote closing with smart context-awareness (won't auto-close inside comments or strings).
  - Smart indentation rules for block scopes (`{}`).

---

## Language Specifications

### Keywords
```Chain
if elif else while for in return break continue try catch import
```

### Storage Types & Declarations
```chain
set func class init new app window package sh
```

### Built-in Support Modules & Functions
- **Modules/Classes**: `print`, `len`, `range`, `math`, `time`, `io`, `os`, `str`, `list`, `fs`, `term`, `dict`, `net`, `audio`, `gui`
- **GUI Functions**: `gui_setup`, `gui_running`, `gui_start`, `gui_present`, `gui_clear`, `gui_rect`, `gui_text`, `gui_close`, `gui_click`, `gui_is_key_pressed`, `gui_is_key_down`, `gui_get_time`

---

## Installation & Development

1. Clone or place this repository into your VSCode extensions directory:
   - Linux: `~/.vscode/extensions/Chain-lang`
2. Open the folder in VSCode.
3. Press `F5` to open a new Extension Development Host window and test your changes.

---

## Extension Structure

- `package.json`: Extension manifest defining language contributions and grammars.
- `Chain.tmLanguage.json`: TextMate grammar rules for tokenization and syntax coloring.
- `language-configuration.json`: Editor behavior rules (brackets, auto-closing pairs, and indentation).
- `launch.json`: Debugging configuration for extension development.

---

## License

GPLv3 License - Part of the **NebulaOS** project.
