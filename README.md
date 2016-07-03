# Sidenotes

Gute Infoquelle: http://alistapart.com/article/get-started-with-git


Folgende Kommandos sind wichtig: 


git clone https://github.com/sam4ritan/kingfisher.git //Erzeugt einen lokalen Ordner des Projekts


git add . //F�gt alle �nderungen dem aktuellen Commit hinzu

git add <Datei1.endung> <Datei2.endung> //Wenn nur bestimmte Dateien commited werden sollen

//git add ist auch n�tig, um neue Dateien der Repo hinzuzuf�gen

git commit -m "Commit Kommentar (Flag)" //Der eigentliche Commit, ohne diesen wird nichts dauerhaft; Bitte immer sinnvoll Kommentieren, das ist ein Wiederherstellungspunkt falls etwas schief l�uft


git commit -a -m "Commit Kommentar (Flag)" //Fasst die beiden Schritte (add und commit) zusammen

git push <repo> <branch> //F�gt die Commits der GitHub Repo hinzu; <repo> ist normalerweise 'origin'; <branch> kann benannt werden, sonnst wird nach einem Branch mit gleichem Namen wie lokal gesucht, sonst kommt es zur Fehlermeldung


git checkout -b <branch> //Erzeugt einen neuen lokalen Branch

git push --set-upstream <repo> <branch> //Erzeugt den neuen Branch in der GitHub Repo und pusht


git fetch //l�dt eventuelle �nderungen von der Repo herunter; --all f�hrt den Befehl f�r alle lokalen Branches durchD

git reset <repo>/<branch> //Zeigt, ob es �nderungen gibt und f�gt NEUE Dateien hinzu

git reset --hard <repo>/<branch> //Setzt den lokalen Branch auf das Niveau der Repo. �BERSCHREIBT ALLE DATEN! Evtl vorher einen neuen lokalen Branch als Backup erstellen



git remote -v //Zeigt derzeitige K�rzel f�r remote Repos (aka. GitHub) an, nur um zu checken, ob alles richtig konfiguriert ist, wenn es zu problemen kommt

git log //Zeigt alle Commits auf aktuellem 

git branch //Zeigt die lokalen Branches an

git checkout //Wechselt lokalen Branch

git rm <Datei.endung> //Entfernt die Datei

git rm --cached <Datei.endung> //Entfernt die Datei in der Repo, bel�sst die lokale Kopie



#Best Practices

1. F�r jedes neue Feature einen separaten Branch erstellen, gemerged wird sp�ter

2. Bei Commit-Konflikten einen neuen Branch erstellen
