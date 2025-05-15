# VSCode

VSCode gibt es in zwei Versionen:
- Onlineversion: [vscode.dev](vscode.dev)
- Desktop version: Download unter [code.visualstudio.com/download](https://code.visualstudio.com/download)


## 1. Visual Studio Code for the Web

**Visual Studio Code** (VS Code) ist ein Code Editor, der keine Installation erfordert, da er vollständig in einem Browserfenster läuft. Sie können damit Quellcode Repositories durchsuchen und auch Änderungen an Quellcodes vornehmen. Sie starten es einfach im Browser mit [vscode.dev](https://vscode.dev).

**VS Code** bietet viele der Features der Desktop Version. Sie können damit sowohl auf Repositories wie z. B. GitHub zugreifen und darauf auch Forks und Pull Request eröffnen,  uns Sie können auch auf lokal gespeicherte Dateien, wie z. B. Ihre Jupyter Notebooks, zugreifen.  

    [Dokumentation](https://code.visualstudio.com/docs/?dv=win64user) 


### Verhältnis zu VS Code Desktop

VS Code for the Web provides a browser-based experience for navigating files and repositories and committing lightweight code changes. However, if you need access to a runtime to run, build, or debug your code, you want to use platform features such as a terminal, or you want to run extensions that aren't supported in the web, we recommend moving your work to the desktop application, GitHub Codespaces, or using Remote - Tunnels for the full capabilities of VS Code. In addition, VS Code Desktop lets you use a full set of keyboard shortcuts not limited by your browser.

When you're ready to switch, you'll be able to "upgrade" to the full VS Code experience with a few clicks.

You can also switch between the Stable and Insiders versions of VS Code for the Web by selecting the gear icon, then Switch to Insiders Version..., or by navigating directly to https://insiders.vscode.dev.
Opening a project

By navigating to https://vscode.dev, you can create a new local file or project, work on an existing local project, or access source code repositories hosted elsewhere, such as on GitHub and Azure Repos (part of Azure DevOps).

You can create a new local file in the web just as you would in a VS Code Desktop environment, using File > New File from the Command Palette (F1).


### GitHub repos

Mit der Anweisung https://vscode.dev/github/<organization>/<repo> können Sie mit **VS Code** direkt ein GitHub Repository öffnen. Um z. B. direkt auf das Repository von Microsoft VS Code zu kommen geben Sie ein https://vscode.dev/github/microsoft/vscode. Um zum Buch-Repository zu gelagen, geben sie im Browser die folgende Sequenz ein [vscode.dev/github/rubinhm/JupyterNBs](https://vscode.dev/github/rubinhm/JupyterNBs)

Mit **VS Code** können Sie somit auf einfache Weise aus der Ferne ein GitHub Repository anschauen und editieren, ohne den Code auf Ihren Computer herunterladen zu müssen. Mehr zu dieser Erweiterung und wie diese genau funktioniert erfahren Sie im *GitHub Repositories guide* (Sie Link oben).

Die GitHub Repository-Erwiterung funktioniert genau so in der Desktop-Version und ermäglicht ihnen ein schnelles Repository-Browsing. Diese Erwiterung müssen Sie natürlich zuerst installieren, dann können Sie ein Repo einfach mit dem Befehl *Open Repository...* öffnen

In Chrome und Edge können Sie Github Repositories auch einfach über das Suchfenster öffnen. Dazu müssen Sie jeweils nur die vscode.dev-Erweiterung installieren.    


## 2. Desktop Version

Falls Ihnen die lokale Installation von Miniconda zu umständlich erscheint und Sie die Erwiterungen von VS Code nicht installieren möchten, können Sie sich die Notebooks von GitHub auf ihren Rechner in einen Ordner herunterladen. Danach können Sie die Notebooks mit der Desktopversion von **VS Code** betrachten, mit ihnen experimentieren und sie direkt in **VS Code** laufen lassen. 




