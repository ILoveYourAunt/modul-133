# Installation der Tools

## Git

Git von https://git-scm.com/ herunterladen und installieren.

#### Git konfigurieren

```bash
git config --global user.name "Priska Meier"
git config --global user.email priska.meier@example.com
```

## Node JS Runtime

Node Version 8.11.x LTS von https://nodejs.org/ herunterladen und installieren.

In der Windows Eingabeaufforderung überprüfen, ob die Installation funktioniert hat:
```bash
node
> 1 + 1
2
> Ctrl-d
```

## Visual Studio Code Editor

Visual Studio Code von https://code.visualstudio.com herunterladen und installieren.

#### Extensions

Die Erweiterungen suchen und installieren.

* Markdown Preview Enhanced
* Live Server

#### Konfiguration

Im Menü `File -> Preferences -> Settings` (`Ctrl`-`,`) nach `enableScriptExecution` suchen, und den Wert der Einstellung auf `true` setzen.