# Export and Import your vscode extensions
To export and import installed extensions in Visual Studio Code, you can use the following commands:
Export extensions:

```bash
code --list-extensions > vscode-extensions.txt
```

This command will create a file called "vscode-extensions.txt" with a list of all installed extensions.
Import extensions:

```bash
cat vscode-extensions.txt | xargs -n 1 code --install-extension
```

This command will read the "vscode-extensions.txt" file and install each listed extension.
For Windows systems, you can use these equivalent commands:
Export:

```bash
code --list-extensions > vscode-extensions.txt
```

Import:

```bash
Get-Content vscode-extensions.txt | ForEach-Object { code --install-extension $_ }
```

These commands are executed from the command line (terminal on macOS/Linux or PowerShell on Windows).

-----

## Spanish

Para exportar e importar las extensiones instaladas en Visual Studio Code, puedes utilizar los siguientes comandos:
Exportar extensiones:

```bash
code --list-extensions > vscode-extensions.txt
```


Este comando creará un archivo llamado "vscode-extensions.txt" con una lista de todas las extensiones instaladas.
Importar extensiones:

```bash
cat vscode-extensions.txt | xargs -n 1 code --install-extension
```

Este comando leerá el archivo "vscode-extensions.txt" e instalará cada extensión listada.
Para sistemas Windows, puedes usar estos comandos equivalentes:
Exportar:

```bash
code --list-extensions > vscode-extensions.txt
```
Importar:

```bash
Get-Content vscode-extensions.txt | ForEach-Object { code --install-extension $_ }
```

Estos comandos se ejecutan desde la línea de comandos (terminal en macOS/Linux o PowerShell en Windows).