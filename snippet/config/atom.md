# Atom Packages

## Customized Packages

### Commont
```shell
#activate-power-mode
atom-beautify
#color-picker
linter
merge-conflicts
#minimap
#open-path
#pigments
project-viewer
repl
#script
terminal-plus / platformio-atom-ide-terminal
vim-mode-plus
```

### Git
```shell
git-log
#git-plus
#git-time-machine
#git-control
```

------

### C/C++
```shell
switch-header-source
autocomplete-clang
clang-format
gpp-compiler
linter-gcc
#language-cpp14
#linter-clang
#linter-cpplint
```

### Go
```
go-outline
go-debug
go-plus
#go-signature-statusbar

## We will use go-guru in future.
## Don't use rubyist/go-oracle, but smo921/go-oracle@branch:guru_cli_args
go-oracle
```

**Configuration**
```shell
$ go install golang.org/x/tools/cmd/guru
```

### JS
```shell
js-hyperclick
#linter-eslint
#language-javascript-jsx
#linter-js-standard
#linter-js-standard-jsx
```

**Configure**
```shell
$ npm install -g eslint
```

### Python
```shell
autocomplete-python
#python-tools
#linter-python-pep257
linter-python-pep8
#linter-python-pyflakes
```

**Configuration**
```shell
pip install pep8 pep257 pylint
```

### Markdown
```shell
language-markdown
```

### SQL
```
qolor
```


## Core Packages
```shell
#about
#archive-view
#autocomplete-atom-api
autocomplete-css
autocomplete-html
autocomplete-plus
autocomplete-snippets
#autoflow
#autosave
#background-tips
bookmarks
bracket-matcher
command-palette
#deprecation-cop
dev-live-reload
encoding-selector
#exception-reporting
find-and-replace
fuzzy-finder
git-diff
go-to-line
grammer-selector
image-view
incompatible-packages
keybinding-resolver
#language-c
#language-clojure
language-coffee-script
#language-csharp
language-css
#language-gfm
language-git
language-go
language-html
language-hyperlink
#language-java
language-javascript
language-json
#language-less
#language-make
#language-mustache
#language-objective-c
#language-perl
#language-php
#language-property-list
language-python
#language-ruby
#language-ruby-on-rails
#language-sass
language-shellscript
language-source
#language-sql
language-text
language-todo
#language-toml
language-xml
language-yaml
line-ending-selector
link
markdown-preview
#metrics
notifications
#open-on-github
#package-generator
settings-view
snippets
#spell-check
status-bar
#styleguide
symbols-view
tabs
timecop
tree-view
update-package-dependencies
#welcome
whitespace
wrap-guide
```

------

# Configuration

## `config.cson`
```cson
"*":
  #"autocomplete-python":
  #  useKite: false
  #  useSnippets: "required"
  #"clang-format":
  #  formatCOnSave: false
  #  formatCPlusPlusOnSave: false
  "command-palette":
    preserveLastSearch: true
  core:
    closeEmptyWindows: false
    disabledPackages: [
      "activate-power-mode"
      "language-gfm"
      "pigments"
      "color-picker"
      "language-javascript-jsx"
      "linter-eslint"
      "minimap"
      "open-path"
      "about"
      "archive-view"
      "autocomplete-atom-api"
      "autoflow"
      "autosave"
      "background-tips"
      "deprecation-cop"
      "exception-reporting"
      "language-c"
      "language-clojure"
      "language-csharp"
      "language-java"
      "language-less"
      "language-make"
      "language-mustache"
      "language-objective-c"
      "language-perl"
      "language-php"
      "language-property-list"
      "language-ruby"
      "language-ruby-on-rails"
      "language-sass"
      "language-sql"
      "language-toml"
      "metrics"
      "open-on-github"
      "package-generator"
      "script"
      "spell-check"
      "styleguide"
      "welcome"
    ]
    openEmptyEditorOnStart: false
    telemetryConsent: "limited"
    themes: [
      "one-light-ui"
      "one-light-syntax"
    ]
  editor:
    autoIndentOnPaste: false
    showIndentGuide: true
    showInvisibles: true
    tabLength: 4
    zoomFontWhenCtrlScrolling: true
  "fuzzy-finder":
    preserveLastSearch: true
  "git-diff":
    showIconsInEditorGutter: true
  linter:
    showErrorTabLine: true
  #"linter-python-pep257":
  #  ignoreCodes: "D100, D101, D102, D103, D104, D105, D209"
  #"linter-python-pep8":
  #  ignoreErrorCodes: "E125, E126, E127, E128, E129, E221, E265, E401"
  "markdown-preview":
    useGitHubStyle: true
  #"markdown-writer":
  #  fileExtension: ".md"
  minimap:
    absoluteMode: true
    plugins:
      cursorline: true
      cursorlineDecorationsZIndex: 0
  #"platformio-ide-terminal":  # Replace terminal-plus
  #  core:
  #    mapTerminalsTo: "Folder"
  #  toggles:
  #    autoClose: true
  "project-viewer":
    convertOldData: false
    hideHeader: true
    keepContext: true
    statusBarVisibility: true
    visibilityState: "Remember state"
  #qolor:
  #  fourBorders: true
  script:
    cwdBehavior: "Project directory of the script"
  tabs:
    enableVcsColoring: true
  "terminal-plus":
    core:
      mapTerminalsTo: "Folder"
    toggles:
      autoClose: true
  "tree-view"
    hideIgnoredNames: true
    hideVcsIgnoredFiles: true
    squashDirectoryNames: true
  "vim-mode-plus":
    clearMultipleCursorsOnEscapeInsertMode: true
    highlightSearch: true
    incrementalSearch: true
    useClipboardAsDefaultRegister: true
  welcome:
    showOnStartup: false
  whitespace:
    ignoreWhitespaceOnCurrentLine: false
```

## `keymap.cson`
```cson
'atom-text-editor':
  'ctrl-a': 'core:select-all'
  'ctrl-x': 'core:cut'
  'ctrl-c': 'core:copy'
  'ctrl-v': 'core:paste'

'atom-workspace':
  'ctrl-a': 'core:select-all'
  'ctrl-x': 'core:cut'
  'ctrl-c': 'core:copy'
  'ctrl-v': 'core:paste'
```
