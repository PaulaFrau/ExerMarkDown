  **Mostra l'historial de canvis del repositori.**

  Git log
    
  **Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt amb el següent text:**
  1. mkadir capitols
  2. cd capitols
  3. nano capitol1.txt
    
  **Afegeix els canvis a la zona d'intercanvi temporal (staging area)**

  git add capitol1.txt
    
  **Fes un commit dels canvis amb el missatge "Afegit capítol 1."**

  git commit -m "Afegit capítol 1."
    
  **Torna a mostrar l'historial de canvis del repositori.**

  Git log

***Exercici 2***

**Crea el fitxer capitol2.txt a la carpeta capítols amb el següent text:**

nano capitol2.txt
    
**Afegeix els canvis a la zona d'intercanvi temporal.**

Git add capitol2.txt
    
**Fes un commit dels canvis amb el missatge "Afegit capítol 2."**

git commit -m "Afegit capítol 2."
    
**Mostra les diferències entre l'última versió i les dues versions anteriors.**

Git diff HEAD^ HEAD
Git diff HEAD^^ HEAD

***Exercici 3***

**Crea el fitxer capitol3.txt a la carpeta capítols amb el següent text:**

nano capitol3.txt
    
**Afegeix els canvis a la zona d'intercanvi temporal.**

Git add capitol3.txt
    
**Fes un commit dels canvis amb el missatge "Afegit capítol 3."**

git commit -m "Afegit capítol 3."
    
**Mostra les diferències entre la primera i l'última versió del repositori.**

git diff $(git rev-list --max-parents=0 HEAD) HEAD

***Exercici 4***

**Afegir al final del fitxer índex.txt la següent línia:**

echo "Afegit capítol 5 a l'índex." >> índex.txt

**Afegir els canvis a la zona d'intercanvi temporal.**

git add índex.txt
    
**Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex."**

git commit -m "Afegit capítol 5 a l'índex."
    
**Mostrar qui ha fet canvis sobre el fitxer índex.txt.**

git blame índex.txt
