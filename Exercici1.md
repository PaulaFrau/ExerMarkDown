***Exercici 1***

**Crea un repositori nou amb el nom llibre i mostra el seu contingut.**
  1. mkadir llibre
  2. cd llibre
  3. git init
  4. ls -a

**Configura Git definint el nom de l'usuari, el correu electrònic i activa l'exida en color. Mostra la configuració final.**
  1. git config --global user.name "Paula Frau"
  2.  git config --global user.email "paula@gmail.com"
  3.  git config --global color.ui "auto"
  4.  git config –list

***Exercici 2***

**Comprova l'estat del repositori.**

  Git status
  
**Crea un fitxer índex.txt amb el següent contingut:**

  sudo nano index.txt
  
**Comprova de nou l'estat del repositori.**

  Git status
  
**Afegeix el fitxer a la zona d'intercanvi temporal.**

  Git add index.txt
  
**Torna a comprovar una vegada més l'estat del repositori.**

  Git status    

***Exercici 3***

**Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i revisa l'estat del repositori.**
  1. git commit -m "Afegit índex del llibre."
  2. git status

***Exercici 4***

**Canvia el fitxer índex.txt perquè continga el següent:**

  nano index.txt
  
**Mostra els canvis respecte a l'última versió guardada al repositori.**

  Git diff
  
**Fes un commit dels canvis amb el missatge "Afegit capítol 3 sobre gestió de branques".**

  1. git add índex.txt
  2. git commit -m "Afegit capítol 3 sobre gestió de branques"

***Exercici 5***

**Mostra els canvis de l'última versió del repositori respecte a l'anterior.**
  1. git log
  2. git diff HEAD^ HEAD
     
**Canvia el missatge de l'últim commit a "Afegit capítol 3 sobre gestió de branques a l'índex."**

  git commit --amend -m "Afegit capítol 3 sobre gestió de branques a l'índex."
  
**Torna a mostrar els últims canvis del repositori.**
  1. git log
  2. git diff HEAD^ HEAD

***Exercici 6***

**Indica a Git que vols ignorar tots els fitxers que comencen per "daw", tots els que tenen l'extensió out i les imatges (jpg, png, bmp i gif).**

  Nano .gitignore
