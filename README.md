# Att använda terminalen (för utveckling)

Första delen med rättigheter, filer, navigering osv finns som quiz i googleforms

* alias
* Variabler, tex: $PATH 

## Filsystemet

## Navigering, filer och mappar
* mv
* du
* file
* find
* grep

## Pipes + operatorer

Läs: https://www.redhat.com/sysadmin/pipes-command-line-linux

`|` (pipe) används för att skicka vidare output från ett verktyg till nästa. Skapa två olika textfiler med kontakter. 

Arbeta med `cat` och `sort`.

```
$ cat contacts.txt

Bob Jones
Leslie Smith
Dana David
Susan Gee
Leonard Schmidt
Linda Gray
Terry Jones
Colin Doe
Jenny Case
Terry Jones
```

```
$ cat kontakter.txt

Jens Berggren
Emil Bengtsson
Johan Eriksson
Lana Ek
Pauline Jakobsson
Nikolina Gustavsson
Linn Forsberg
```

Hur kan du:
* sortera en lista?
* spara den sorterade listan?
* sortera på efternamn?
* vända sorteringen?
* slå ihop och sortera namnen från både contacts.txt och kontakter.txt

Vad gör kommandot: `cat contacts.txt | sort | uniq` ?

---





### Standard streams: stdin / stdout / stederr
Tydlig guide, svår: https://www.howtogeek.com/435903/what-are-stdin-stdout-and-stderr-on-linux/

## Loggfiler

## Brew

## Rättigheter (i filsystemet)

* filrättigheter (ls -l / chmod)
* användare - grupper (chown / chgrp)
* root - sudo

Bra men svår guide om rättigheter: https://help.ubuntu.com/community/FilePermissions 