# Übung: Workflows

## Übung 1: Erster Workflow

1. Forken Sie dieses Repository, um eine beispielhafte Implementierung zu erhalten. 
1. Erstellen Sie dann einen **Frontend** Workflow, der: 
	1. Ausgeführt wird, sobald Änderungen in Ihrem Repository erkannt werden.
	1. Den Inhalt des Repository ins Arbeitsverzeichnis lädt.
	1. Den Inhalt der Datei `src/frontend/app.js` auf die Konsole druckt.
1. Testen Sie Ihren Workflow, indem Sie die Konfigurationsdatei in das Repository pushen.


## Übung 2: Frontend und Backend Build

1. Erweitern Sie den **Frontend** Workflow, sodass er: 
	1. Nach dem Checkout Node.js initialisiert und `node src/frontend/app.js` ausführt.
	1. Die Datei `src/frontend/app.js` in den neuen Ordner `dist` kopiert und dabei eine Kommentarzeile (`//`) als erste Zeile in die Datei einfügt. Diese sollte den Zeitpunkt des Build enthalten.
	1. Statt `src/frontend/app.js` nun `dist/app.js` ausführt, um einen Test zu simulieren.
1. Erstellen Sie dann einen **Backend** Workflow, der das Backend in gleicher Weise baut und testet: 
	1. Herunterladen des Repository Inhalts, Initialisierung von Python und Erstellen des dist Ordners.
	1. Kopieren der Datei `src/backend/run.py`. Dabei Einfügen einer Kommentarzeile (`#`) mit Zeitpunkt des Build. Abschließend Ausführen von `python dist/run.py` zum Test.
