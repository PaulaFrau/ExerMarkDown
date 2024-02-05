***Exercici 1***

**Elimina l'última línia del fitxer índex.txt i guarda-ho.**

sed -i '$d' índex.txt

**Comprova l'estat del repositori.**

Git status

**Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.**

git checkout -- índex.txt

**Torna a comprovar l'estat del repositori.**

Exercici 2

**Elimina l'última línia del fitxer índex.txt i guarda-ho.**

sed -i '$d' índex.txt

**Afegeix els canvis a la zona d'intercanvi temporal.**

Git add index.txt

**Comprova de nou l'estat del repositori.**

Git status
  
**Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.**

Git reset HEAD index.txt

**Comprova de nou l'estat del repositori.**

Git status

**Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.**

git checkout -- índex.txt

**Torna a comprovar l'estat del repositori.**
Git status

***Exercici 3***

**Elimina l'última línia del fitxer índex.txt i guardar-ho.**

sed -i '$d' índex.txt

**Elimina el fitxer capítols/capitol3.txt.**

rm capitol3.txt

**Afegeix un fitxer nou capítols/capitol4.txt buit.**

touch capitol4.txt

**Afegeix els canvis a la zona d'intercanvi temporal.**

git add índex.txt capitol4.txt

**Comprova de nou l'estat del repositori.**

**Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.**

git reset HEAD index.txt capitol4.txt
 
**Comprova de nou l'estat del repositori.**

Git status

**Desfés els canvis realitzats per tornar a la versió del repositori.**

git checkout -- index.txt capitol4.txt

**Torna a comprovar l'estat del repositori.**

***Exercici 4***

**Elimina l'última línia del fitxer índex.txt i guardar-ho.**

sed -i '$d' índex.txt

**Elimina el fitxer capítols/capitol3.txt.**

Rm capitol3.txt

**Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Borrat accidental."**

git commit -m "Borrat accidental."

**Comprova l'historial del repositori.**

Git log

**Desfés l'últim commit, però mantin els canvis anteriors al directori de treball i a la zona d'intercanvi temporal.**

Git reset HEAD^

**Comprova l'historial i l'estat del repositori.**
1. git log
2. git status

**Torna a fer el commit amb el mateix missatge d'abans.**

git commit -c ORIG_HEAD

**Desfés l'últim commit i els canvis anteriors al directori de treball, tornant a la versió anterior del repositori.**

git reset --hard ORIG_HEAD

**Comprova de nou l'historial i l'estat del repositori.**
1. git log
2. git status
 
