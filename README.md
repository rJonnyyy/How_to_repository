großes kleines git tutorial:

für Rust:

cargo new file 
* .git versteckter Ordner wird bereits automatisch mit cargo new file generiert 

* git init (eigentlich muss im Verzeichnis wo das Repo erstellt werden soll cmd >> git init >> git add . (all) gemacht werden)
* git add . (vll auch nicht)
** werden somit bereits erledigt

-----------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------

1. Schritt: Remote repository auf github.com erstellen
--> WICHTIG: ** Keine README.md erzeugen, sonst kommt es zu Problemen, dass remote und lokal repo unterschiedlich sind 



2. git bash in neuem rust ordner projekt öffnen 

* git remote add origin URL <HTTPS>
--> mögliche Fehler: git remote -v >> git remote remove origin 

* git add .

* git commit -m "first commit"

* git push -u origin main (Standardmäßig auf main pushen)
--> jetzt ist sind alle rust files im github repo 


3. README.md erstellen

* im Rust ordner README.md aus textdokument erstellen

* git add README.md 

* git commit -m "Add README.md files"

* git push

-----------------------------------------------------------------------------------------------------------------------------

4. Erstellung beendet 
--> Ab jetzt nach jeder Änderung der main.rs

git add src/main.rs
git commit -m "Änderung"
git push 


-----------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------

Hier sind einige der wichtigsten Git-Befehle mit einer kurzen Beschreibung:

- git init:
Initialisiert ein neues Git-Repository in einem Verzeichnis. Dadurch wird ein .git-Verzeichnis erstellt, das für das Versionsmanagement verwendet wird.

- git clone URL<repository-url>:
Klont ein vorhandenes Git-Repository von einer Remote-URL und erstellt eine lokale Kopie des Repositories auf Ihrem Computer.

- git add file<file>:
Fügt eine Datei oder Änderungen an einer Datei zum Index (Staging-Bereich) hinzu, um sie für den nächsten Commit vorzubereiten.

- git commit -m "<commit-message>":
Committet die im Index befindlichen Änderungen in das lokale Repository. Die Nachricht "msg"<commit-message> beschreibt die durchgeführten Änderungen.

- git status:
Zeigt den Status des Arbeitsverzeichnisses und des Index an. Dies umfasst Informationen über unversionierte, geänderte oder zum Commit vorgemerkte Dateien.

- git push:
Überträgt lokale Commits zum Remote-Repository, sofern es mit einem Upstream-Branch verknüpft ist. Es wird normalerweise verwendet, um lokale Änderungen mit anderen zu teilen.

- git pull:
Holt Änderungen vom Remote-Repository und fusioniert sie mit dem lokalen Branch. Es ist eine Kombination aus git fetch (Herunterladen der Änderungen) und git merge (Zusammenführen der Änderungen).

- git fetch:
Holt Änderungen vom Remote-Repository, lädt sie jedoch nicht automatisch in den Arbeitsbereich. Es ermöglicht Ihnen, die neuesten Änderungen zu sehen, ohne sie sofort zu integrieren.

- git merge "branch/main"<branch>:
Fusioniert den angegebenen Branch in den aktuellen Branch. Dies wird verwendet, um Änderungen von einem anderen Branch in den aktuellen Branch zu übernehmen.

- git branch:
Zeigt eine Liste der vorhandenen Branches an oder erstellt einen neuen Branch, wenn ein Name angegeben ist. Es wird auch verwendet, um zwischen Branches zu wechseln.

- git checkout "branch/main"<branch>:
Wechselt zwischen verschiedenen Branches. Es kann auch verwendet werden, um eine bestimmte Datei aus einem anderen Branch wiederherzustellen.

- git log:
Zeigt eine Liste der Commits im aktuellen Branch an, einschließlich Informationen wie Autor, Datum und Commit-Nachricht.

Diese Befehle bilden eine grundlegende Grundlage für die Verwendung von Git und sind entscheidend für das Arbeiten mit einem Git-Repository.


-----------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------


* danger zone / repo löschen 

cd repository_Verzeichnis -->

Stelle sicher, dass du im richtigen Repository bist:
* git status

Um das Repository von GitHub zu löschen, verwende den Befehl 
* git remote rm origin --> Dadurch wird die Verbindung zum entfernten Repository entfernt.

Als nächstes lösche das lokale Repository. Du kannst dazu den Befehl 
* rm -rf .git verwenden. 
--> Beachte dabei, dass dies das gesamte Git-Verzeichnis löscht, einschließlich aller Commits, Branches und Konfigurationen.

!! Nun musst du noch das Repository auf GitHub selbst löschen. Dies kannst du über die GitHub-Website oder über die GitHub-API tun.

Über die Website:

Gehe auf die GitHub-Website und melde dich in deinem Konto an.
Gehe zu dem Repository, das du löschen möchtest.
Klicke auf "Settings" (Einstellungen) in der oberen rechten Ecke.
Scrolle nach unten zu "Danger Zone" (Gefahrenzone).
Klicke auf "Delete this repository" (Dieses Repository löschen).
Gib den Namen des Repositorys zur Bestätigung ein.
Klicke auf "I understand the consequences, delete this repository" (Ich verstehe die Konsequenzen, dieses Repository löschen).








