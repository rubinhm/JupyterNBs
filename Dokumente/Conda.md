# Miniconda  und Qiskit lokal einrichten

Conda ist ein recht leistungsstarkes Kommandozeilen-Programm für das Management von Softwareumgebungen. Es ist kostenlos erhältlich für Windows macOS und Linux. Hier wird Schritt für Schritt erklärt, wie Sie mit Miniconda  Qiskit und Jupyter Lab auf Ihrem Rechner lokal eine minimale Umgebung zur Bearbeitung der Jupyter Notebooks zum Buch einrichten können. Ausführlichere Beschreibungen erhalten Sie von der Website [Getting started wirh conda](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html).

Qiskit ist ein auf der Programmiersprache Python basierendes Software Entwicklungspaket (SDK) von IBM. Minikonda ist ein Software Paketmanager, der bereits Python enthält. Deshalb muss zuerst Miniconda installiert werden. Damit kann dann das Jupyter Lab und anschliessend Qiskit installiert werden. Mit dem Jupyter Lab können die Notebooks zu diesem Buch laufen gelassen und editiert werden.

Seit der Drucklegung dieses Buches haben sich die Plattformen (IBMQ, Qiskit und Python) weiterentwickelt. Die zur Drucklegung dieses Buches entwickelten Jupyter Notebooks laufen bereits mit den neuesten Versionen von Qiskit und Pythtn nicht mehr fehlerfrei. 

Anstatt die Notebooks ständig den neuesten Softwareversionen anzupassen, ist es einfacher diejenigen Versionen von Python und Qiskit zu installieren, mit denen die Notebooks stabil laufen. Zur Installation verwenden wir hier Minikonda3 in der Version mit Python 3.11.11 Diese Version kann unter [https://repo.anaconda.com/miniconda/](https://repo.anaconda.com/miniconda/){:target="_blank"} heruntergeladen werden. Es stehen Versionen für Windows, macOS und Linux zur verfügung. Für Windows und ein 64-Bit System suchen Sie Miniconda3-py311_25.3.1-1-Windows-x86_64.exe in der Liste und laden dieses Installationsprogramm auf ihren Rechner. Die folgenden Installationsschritte gelten für eine Neuinstallation ohne vorherige Versionen von Python und Qiskit.

## Installationsschritte

1. Führen Sie das heruntergeladene Installationsprogramm aus.
2. Nach der Installation suchen Sie das Konsolenprogramm Anaconda Prompt (miniconda 3) oder Anaconda PowerShell. Dies sind die Konsolen für die Eingabe der weiteren Befehle. In der Eingabezeile sehen Sie (base)...
3. Installieren Sie das Jupyter Lab in (Base): pip install jupyterlab / falls pip nicht installiert ist: conda install -c conda-forge jupyterlab
4. (Nur falls  der Python Paketmanager pip nicht vorhanden sein sollte, installieren Sie ihn jetzt mittels: conda install pip)
5. Nun wird die gewünschte Qiskit-Version installiert. Wir wählen: pip install qiskit==0.43.1
6. Nun benötigen wir noch weitere Module für die verschiedenen Visualisierungen und die Verbindung zu IBM Quantum:
   - *MatPlotLib* Installation mittels: pip install matplotlib
   - *PyLatexEnc* Installation mittels: pip install pylatexenc
   - *Seaborn* Installation mittels: pip install seaborn
   - *IBM Runtime* Installation mittels: pip install qiskit_ibm_runtime. (Die Qiskit-IBM-Runtime benötigen Sie nur, falls Sie Ihre Schaltkreise auf einen IBM-Quantencomputer ausführen wollen. Für die Beispiele im Buch genügt ein Simulator, wie z. B. der QASM-Simulator.)
7. Starten Sie schliesslich das Jupyter Lab (mit start jupyter lab). Danach wird das Jupyter Lab in einem Browswerfenster geladen.

Falls Sie die neueste Version von Anaconda Navigator oder Miniconda3 heunterladen wollen, gehen Sie auf: [www.anaconda.com/download](https://www.anaconda.com/download){:target="_blank"}
Hier muss man eine E-Mail Adresse eingeben, damit es weiter geht. Anschliessend kann man die gewünschte Installation wählen (Windowa, Mac, Linux).

**Wichtig:** eine andere Python- und Qiskit-Version sollten Sie in einer neuen virtuellen Umgebung installieren. In Jupyter Lab können Sie dann jeweils Version (Kernel) wählen.

## Erstellen einer virtuellen Umgebung

Eine virtuelle Umgebung benötigen Sie, falls Sie eine neuere Version von Python oder Qiskit installieren wollen oder falls Sie bereits eine Python und Qiskit Version installiert haben, müssen Sie die oben angegebenen Schritte in dieser neuen virtuellen Umgebung ausführen.
Dazu geben Sie in Ihrer (base)-Umgebung ein: conda create --name  '*Umgebungsname*'.
 '*Umgebungsname*' ersetzen Sie durch den von Ihnen gewählten Namen. Im Installationsverzeichnis /miniconda3/envs/wird ein Ordner für Ihre virtuelle Umgebung mit dem von Ihnen gewählten Namen (*Umgebungsname*) erstellt.
- Um in Ihre Umgebung zu kommen, geben Sie am Prompt ein: activate *Umgebungsname*. Vor dem Prompt sehen Sie jetzt in runden Klammern ihre Umgebung (*Umgebungsname*)


## Anleitungen aus dem Web

[Getting started with conda](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html){:target="_blank"}

[Installationsvideo](https://www.anaconda.com/docs/getting-started/miniconda/install){:target="_blank"}


## Probleme

Mit dieser Installation wird die neueste Qiskit-Version installiert (>2.0.0). Ab Version 1 werden gewisse Funktionen nicht mehr unterstützt, wie z. B. execute oder BasicAer.
Siehe dazu [docs.quantum.ibm.com/migration-guides/qiskit-1.0-features](https://docs.quantum.ibm.com/migration-guides/qiskit-1.0-features){:target="_blank"}

Die in diesem Repository enthaltenen Notbooks laufen gut unter Qiskit bis Version 0.43. Ab Version >1 bitte den o. g. Migrationsguide beachten. Vielleicht hilft ggf. auch dieser [Link](https://schrodinteq.github.io/venv/){:target="_blank"} weiter. Er beschreibt, wie man die Version 0.43 von Qiskit installieren kann.


