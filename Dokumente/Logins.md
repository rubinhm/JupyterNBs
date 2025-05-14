# Miniconda  und Qiskit lokal einrichten

Qiskit ist ein auf der Programmiersprache Python basierendes Software Entwicklungspaket (SDK) von IBM. Minikonda ist ein Software Paketmanager, der bereits Python enthält. Deshalb muss zuerst Miniconda installiert werden. In Miniconda kann dann Qiskit und anschliessend das Jupyter Lab installiert werden. Mit dem Jupyter Lab können die Notebooks zu diesem Buch laufen gelassen und editiert werden.

Seit der Drucklegung dieses Buches haben sich die Platformen (IBMQ, Qiskit und Python) weiterentwickelt. Die zur Drucklegung dieses Buches entwickelten Jupyter Notebooks laufen bereits mit den neuesten Versionen von Qiskit und Pythtn nicht mehr fehlerfrei. 

Anstatt die Notebooks ständig den neuesten Softwareversionen anzupassen, ist es einfacher diejenigen Versionen von Python und Qiskit zu installieren, mit denen die Notebooks stabil laufen. Zur Installation verwenden wir hier Minikonda3 in der Version mit Python 3.11. Diese Version kann unter [https://repo.anaconda.com/miniconda/](https://repo.anaconda.com/miniconda/) heruntergeladen werden. Es stehen Versionen für Windows, MacOS und Linux zur verfügung. Für Windows und ein 64-Bit System suchen Sie Miniconda3-py311_25.3.1-1-Windows-x86_64.exe und laden dieses Installationsprogramm auf ihren Rechner.


- Download Link: [www.anaconda.com/download](https://www.anaconda.com/download)
Hier muss man eine E-Mail Adresse eingeben, damit es weiter geht. Anschliessend kann man die gewünschte Installation wählen (Windowa, Mac, Linux)

- Nach der Installation startet man Anaconda Prompt (miniconda 3). Dies ist die Konsole für die Eingabe der weiteren Befehle.
- Es wird empfohlen, zuerst eine virtuelle Umgebung einzurichten. Dazu gibt man ein: conda create --name  '*Umgebungsname*'.
 '*Umgebungsname*' ersetzen Sie durch den von Ihnen gewählten Namen. Im Installationsverzeichnis /miniconda3/envs/wird ein Ordner für Ihre virtuelle Umgebung mit dem von Ihnen gewählten Namen (*Umgebungsname*) erstellt.
- Um in Ihre Umgebung zu kommen geben Sie am Prompt ein: activate *Umgebungsname*. Vor dem Prompt sehen Sie jetzt in runden Klammern ihre Umgebung (*Umgebungsname*)
- Jetzt kann das Jupyter Lab installiert werden mit der Eingabe: conda install -c conda-forge jupyterlab
- Nun muss das Paketinstallationsprogramm von Python (pip) instaliert werden, mit der Eingabe: conda install pip
- Damit lässt sich jetzt Qiskit installieren: pip install qiskit==0.44.1
- Für die Visualisierungen benötigen Sie noch die Bibliothek *MatPlotLib*. Installation mittels: pip install matplotlib
- ausserdem pip install pylatexenc

Um Jupyter Lab zu starten, starten sie die Konsole Anaconda Prompt, wechseln in ihre virtuelle Umgebung (mit activate ...) und starten anschliessend das Jupyter Lab (mit start jupyter lab). Danach wird das Jupyter Lab in einem Browswerfenster geladen.

## Anleitungen aus dem Web

[Getting started with conda](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html)

[Installationsvideo](https://www.anaconda.com/docs/getting-started/miniconda/install)


## Probleme

Mit dieser Installation wird die neueste Qiskit-Version installiert (>2.0.0). Ab Version 1 werden gewisse Funktionen nicht mehr unterstützt, wie z. B. execute oder BasicAer.
Siehe dazu [docs.quantum.ibm.com/migration-guides/qiskit-1.0-features](https://docs.quantum.ibm.com/migration-guides/qiskit-1.0-features)

Die in diesem Repository enthaltenen Notbooks laufen gut unter Qiskit bis Version 0.46. Ab Version >1 bitte den o. g. Migrationsguide beachten.

Vielleicht bringt dieser [Link](https://schrodinteq.github.io/venv/) eine Lösung. Er beschreibt, wie man die Version 0.46 von Qiskit installieren kann.


