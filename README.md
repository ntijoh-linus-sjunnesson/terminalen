# Att använda terminalen (för utveckling)

Första delen med rättigheter, filer, navigering osv finns som quiz i googleforms.

Todo:
* alias
* Variabler, tex: $PATH 

## Filsystemet
Todo

## Navigering, filer och mappar
Todo:
* mv
* du
* file
* find

## Pipes + operatorer

Läs: https://www.redhat.com/sysadmin/pipes-command-line-linux

`|` (pipe) används för att skicka vidare output från ett verktyg till nästa. Skapa två olika textfiler med kontakter. Arbeta med `cat`, `sort` och `grep`.

Exempelfiler

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

### Övningar: pipes och operatorer

* Hur kan du sortera en lista?
* Hur sparar du den sorterade listan?
* Hur sorterar du på efternamn?
* Hur kan du vända sorteringen?
* Hur kan du slå ihop och sortera namnen från både contacts.txt och kontakter.txt
* Hur kan du söka bland båda listorna?
* Vad gör kommandot: `cat contacts.txt | sort | uniq` ?

### Standard streams: stdin / stdout / stederr

Output från terminalen 

Läs: https://www.redhat.com/sysadmin/redirect-operators-bash och för att fördjupa kunskaperna: https://www.howtogeek.com/435903/what-are-stdin-stdout-and-stderr-on-linux/

## Loggfiler

* tail
* head

## Brew

## Rättigheter (i filsystemet)

* filrättigheter (ls -l / chmod)
* användare - grupper (chown / chgrp)
* root - sudo

Bra men svår guide om rättigheter: https://help.ubuntu.com/community/FilePermissions 