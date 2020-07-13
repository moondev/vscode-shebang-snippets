# Shebang Snippets

[![Visual Studio Marketplace](https://img.shields.io/vscode-marketplace/v/rpinski.shebang-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=rpinski.shebang-snippets)

Set of snippets for [Visual Studio Code](https://code.visualstudio.com/) to insert "shebang" lines for various types of scripts and interpreters used on Unix-like systems.

## Features

After opening a new file you can just type:

- `#!` or `shebang` if the file type is detected
    ![Shebang Snippets in action](https://user-images.githubusercontent.com/1767539/31865808-113720ae-b775-11e7-9267-e9c722ef4ac2.png)
    Note: For most of the supported languages `#` means the beginning of a comment, so there you always have to press `CTRL` + `SPACE` after `#!` to see the snippet due to VSCode behavior with comments.
- `#!` and the interpreter name if the file type is **NOT** detected
    ![Shebang Snippets in action](https://raw.githubusercontent.com/Rpinski/vscode-shebang-snippets/master/images/snippet.gif)

to add the full line. Currently supported shebang snippets:

- Shell:
  - `#!sh` -> `#!/usr/bin/env sh`
  - `#!bash` -> `#!/usr/bin/env bash`
- Expect: `#!expect` -> `#!/usr/bin/expect -f`
- Perl: `#!perl` -> `#!/usr/bin/env perl`
- Lua: `#!lua` -> `#!/usr/bin/env lua`
- Python:
  - `#!python` -> `#!/usr/bin/env python`
  - `#!python+encoding` ->
    - `#!/usr/bin/env python`
    - `# -*- coding: utf-8 -*-`
- PHP: `#!php` -> `#!/usr/bin/env php`
- Node: `#!node` -> `#!/usr/bin/env node`
- F#: `#!fsharp` -> `#!/usr/bin/env fsharpi --exec`
- Ruby:
  - `#!ruby` -> `#!/usr/bin/env ruby`
  - `#!ruby+encoding` ->
    - `#!/usr/bin/env ruby`
    - `# -*- coding: utf-8 -*-`
- Groovy: `#!groovy` -> `#!/usr/bin/env groovy`
- PowerShell Core: `#!pwsh` or `#!powershell` -> `#!/usr/bin/env pwsh`

To insert the magic comment for encoding (`# -*- coding: utf-8 -*-`) you can also just type `#encoding`. The snippet offers different encodings for selection.

If you have already saved your script with appropriate file extension and need the shebang, you can alternatively just start typing `shebang` to complete the line for your script type.
