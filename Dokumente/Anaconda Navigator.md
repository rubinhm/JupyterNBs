# Anaconda Navigator

Falls Sie mit der Minimalen Umgebung von Miniconda und mit der Kommadozeile nicht zurecht kommen oder die Sache nicht richtig funktioniert, empfehlen wir die Instalation von Anaconda Navigator. Dabei handelt es sich um eine umfangreiche Softwareumgebung für wissenschaftliche Anforderungen. Darin enthalten sind **Python** und auch das **Jupyter Lab**, sowie vieles mehr, das Sie wahrscheinlich nicht brauchen, falls Sie sich nur mit den Jupyter Notebooks des Buches befassen wollen. 

Zum Download kommen Sie via [www.anaconda.com/download](https://www.anaconda.com/download). Hier müssen Sie zunächst eine E-Mail Adresse angeben, danach kommen Sie zur Downloadseite.

Hier wählen Sie unter Distribution Installers die für Ihr Betriebssystem passende Version aus. Das Installationsprogramm umfasst über 900 MB, das Sie nach der Installation wieder löschen können.

Führen Sie das Installationsprogramm aus, wird die aktuelle Version von anaconda3 auf Ihrem Rechner installiert. Notieren Sie sich den Installationspfad. 

Wenn Sie den Navigator zum ersten Mal starten, werden Sie ggf. zu einem Update auf die neueste Version verwiesen. Diese wird dringend empfohlen.

Starten Sie den Navigator erneut. In der linken Spalte sehen Sie die Punkte Home, Environments, Learning und Community.

- Unter Home sehen Sie die Installierten Programme (zunächst in der base-Umgebung)
- Unter Environments sehen Sie zunächst nur die aktuelle Umgebung base(root), in der die aktuelle Python-Version installiert ist. Die Buch-Notebooks laufen fehlerfrei unter der Python-Version 3.11.11. Deshalb müssen Sie fafür eine neue virtuelle Umgebung erzeugen.
- Mit der [+]-Schaltfläche unten in dieser Spalte können Sie nun die neue virtuelle Umgebung erzeugen. Im darauf erscheinenden Dialogfeld geben Sie den Namen der neuen Umgebung ein und wählen die Python-Version (3.11.11). Danach wird Ihre neue Umgebung in der der Spalte aufgelistet.
- Je nach Bedarf kann hier zwischen den virtuellen Umgebungen umgeschaltet werden.
- In der neu erstellten Umgebung installieren Sie den *Powershell Prompt* oder/und den *Anaconda Prompt* sowie *Jupyter Lab*.
- *Powershell Prompt* und *Anaconda Prompt* sind zwei Kommandozeilen-Programme. In denen Sie die weiteren Befehle eingeben müssen. Hier installieren Sie die für uns wichtige Qiskit-Version 0.43.1 sowie die weiteren erforderlichen Module gemäss folgender Liste:
    - `pip install qiskit==0.43.1`
    - `pip install matplotlib`
    - `pip install pyltexenc`
    - `pip install seaborn`

Falls Sie beabsichtigen, Ihre Schaltkreise auf einem IBM Quantencomputer laufen zu lassen, installieren Sie abschliessen (oder später) die ibm.runtime mit `pip install qiskit-ibm-runtime`.


 

