großes kleines git tutorial:

für Rust:

cargo new file 
* .git versteckter Ordner wird bereits automatisch mit cargo new file generiert 

* git init 
* git add . (vll auch nicht)
** werden somit bereits erledigt

-----------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------

1. Schritt: Remote repository auf github.com erstellen
--> WICHTIG: ** Keine README.md erzeugen, sonst kommt es zu Problemen, dass remote und lokal repo unterschiedlich sind 



2. git bash in neuem rust ordner projekt öffnen 

* git remote add origin <HTTPS>
--> mögliche Fehler: git remote -v >> git remote remove origin 

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