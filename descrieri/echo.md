#Comanda echo

În sistemul de operare Linux comanda **echo** este folosită pentru a tipări un text specificat pe linia de comandă sau, adesea, în scripturi.

####Sintaxă

`echo [opțiune(i)] [string(s)]`

Un string reprezintă o secvență de caractere(de exemplu: litere, numere etc).

####Mod de utilizare

Comanda echo, folosită fară alte opțiuni sau stringuri returnează o linie goală pe ecran urmată de linia de comandă, un rând mai jos.
Acest lucru se întâmplă deoarece tasta ENTER transmite sistemului comanda de a începe o nouă linie, dar și să execute comanda respectivă.
Dacă trimitem un string drept argument, comanda echo repetă acel string pe ecran astfel:

`$ echo Acesta este un exemplu`

`Acesta este un exemplu`

De remarcat faptul că nu este necesară folosirea ghilimelelor, dacă ele sunt totuși folosite, ele nu vor apărea pe ecran.

`$ echo 'bcjdscbaslc'`

`bcjdscbaslc`

Putem, de exemplu, crea o variabilă x și să îi setăm o valoare, astfel ca ea va putea fi tipărită folosind comanda echo:

`$ echo Valoarea variabilei x este $x`

`Valoarea variabilei x este 10`

În plus, echo poate fi folosită și pentru a indica valoarea variabilelor de mediu:

`$ echo $PATH`

`/usr/lib/lightdm/lightdm:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games`

####Opțiuni

Cele mai folosite opțiuni sunt:

* `-n` : Mesajul nu este afișat pe un rând nou. (ignoră ENTER);
* `-e` : Este folosită pentru a putea recunoaște unele secvențe ce urmează după caracterul backslash;
* `-E` : Dezactivează opțiunea anterioara, -e;
* `--help` : Afișează un mesaj  de ajutor;
* `--version` : Afișează informații despre versiune.

În cazul în care se specifică opțiunea **-e**, următoarele secvențe vor fi recunoscute:

* `\\` : Caracterul backslash;
* `\a` : Alertă;
* `\b` : Backspace;
* `\c` : Comentariu, după acest caracter nu se mai tipărește;
* `\e` : Caraterul ESCAPE;
* `\n` : Linie nouă;
