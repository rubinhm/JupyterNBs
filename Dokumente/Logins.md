# Qiskit und Miniconda

- Download Link: [www.anaconda.com/download](https://www.anaconda.com/download)
Hier muss man eine E-Mail Adresse eingeben, damit es weiter geht. Anschliessend kann man die gewünschte Installation wählen (Windowa, Mac, Linux)

- Nach der Installation startet man Anaconda Prompt (miniconda 3). Dies ist die Konsole für die Eingabe der weiteren Befehle.
- Es wird empfohlen, zuerst eine virtuelle Umgebung einzurichten. Dazu gibt man ein: conda create --name  '*Umgebungsname*'.
 '*Umgebungsname*' ersetzen Sie durch den von Ihnen gewählten Namen. Im Installationsverzeichnis /miniconda3/envs/wird ein Ordner für Ihre virtuelle Umgebung mit dem von Ihnen gewählten Namen (*Umgebungsname*) erstellt.
- Um in Ihre Umgebung zu kommen geben Sie am Prompt ein: activate *Umgebungsname*. Vor dem Prompt sehen Sie jetzt in runden Klammern ihre Umgrbung (*Umgebungsname*)
- Jetzt kann das Jupyter Lab installiert werden mit der Eingabe: conda install -c conda-forge jupyterlab
- Nun muss das Paketinstallationsprogramm von Python (pip) instaliert werden, mit der Eingabe: conda install pip
- Damit lässt sich jetzt Qiskit installieren: pip install qiskit
- Für die Visualisierungen benötigen Sie noch die Bibliothek *MatPlotLib*. Installation mittels: pip install matplotlib

Um Jupyter Lab zu starten, starten sie die Konsole Anaconda Prompt, wechseln in ihre virtuelle Umgebung (mit activate ...) und starten anschliessend das Jupyter Lab (mit start jupyter lab). Danach wird das Jupyter Lab in einem Browswerfenster geladen.

## Probleme

Mit dieser Installation wird die neueste Qiskit-Version installiert (>2.0.0). Ab Version 1 werden gewisse Funktionen nicht mehr unterstützt, wie z. B. execute oder BasicAer.
Siehe dazu [docs.quantum.ibm.com/migration-guides/qiskit-1.0-features](https://docs.quantum.ibm.com/migration-guides/qiskit-1.0-features)

Die in diesem Repository enthaltenen Notbooks laufen gut unter Qiskit bis Version 0.46. Ab Version >1 bitte den o. g. Migrationsguide beachten.

Vielleicht bringt dieser [Link](https://schrodinteq.github.io/venv/) eine Lösung. Er beschreibt, wie man die Version 0.46 von Qiskit installieren kann.


