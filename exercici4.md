***Exercici 1***

**Crea una nova branca bibliografia i mostrar les branques del repositori.**
1. git branch bibliografia
2. git branch

***Exercici 2***

**Crear el fitxer capítols/capitol4.txt i afegir el següent text**
1. cd capitols
2. nano capitol4.txt

**Afegir els canvis a la zona d'intercanvi temporal.**

Git add capitol4.txt

**Fer un commit amb el missatge "Afegit capítol 4."**

git commit -m "Afegit capítol 4."

**Mostrar la història del repositori incloent totes les branques.**

git log --all --graph --oneline

***Exercici 3***

**Canvia a la branca bibliografia.**

git checkout bibliografia

**Crea el fitxer bibliografia.txt i afegir la següent referència:**

nano bibliografia.txt

**Afegeix els canvis a la zona d'intercanvi temporal.**

Git add bibliografia.txt

**Fes un commit amb el missatge "Afegida primera referència bibliogràfica."**

git commit -m "Afegida primera referència bibliogràfica."

**Mostra la història del repositori incloent totes les branques.**

git log --all --graph --oneline

***Exercici 4***

**Fusiona la branca bibliografia amb la branca master.**
1. git checkout master
2. git merge bibliografia

**Mostra la història del repositori incloent totes les branques.**

git log --all --graph –oneline

**Elimina la branca bibliografia.**

git branch -d bibliografia

**Mostra de nou la història del repositori incloent totes les branques.**

git log --all --graph –oneline

***Exercici 5***

**Crea la branca bibliografia.**

git branch bibliografia

**Canvia a la branca bibliografia.**

git checkout bibliografia

**Canvia el fitxer bibliografia.txt perquè continga les següents referències:**

nano bibliografia.txt

**Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."**
1. git add bibliografia.txt
2. git commit -m "Afegida nova referència bibliogràfica."

**Canvia a la branca master.**

git checkout master

**Canvia el fitxer bibliografia.txt perquè continga les següents referències:**

nano bibliografia.txt

**Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."**

1. git add bibliografia.txt
2. git commit -m "Afegida nova referència bibliogràfica."

**Fusiona la branca bibliografia amb la branca master.**

git merge bibliografia

**Resol el conflicte deixant el fitxer bibliografia.txt amb les referències:**

nano bibliografia.txt

**Afegeix els canvis a la zona d'intercanvi temporal i fes un commit amb el missatge "Resolt conflicte de bibliografia."**
1. git add bibliografia.txt
2. git commit -m "Resolt conflicte de bibliografia."

**Mostra la història del repositori incloent totes les branques.**

git log --all --graph –oneline
