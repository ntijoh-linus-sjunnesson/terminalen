# Att använda terminalen (för utveckling)

Första delen med rättigheter, filer, navigering osv finns som quiz i googleforms. Todo: Flytta in det hit.

Kommandot alias skapar en genväg till kommandon, med eller utan nycklar, för att t.ex. spara tid. Exempel.
```
$ alias lista="ls -lah
$ lista
```

Todo:
* ln - länkar - hårda och mjuka
* Variabler, tex: $PATH 

## Filsystemet

En kortfattad beskrivning av Unix-filsystemet:
```
/var/log - loggfiler
/etc - inställningar + startup scripts
/proc - hårdvaruinfo. om tex. cpu osv
/dev - enheter
/home - alla användares hemmappar
```
För djupare förståelse läs: https://tldp.org/LDP/sag/html/dir-tree-overview.html 

## Navigering, filer och mappar

Läs: https://www.fosslinux.com/43292/linux-terminal-commands-to-try-for-a-beginner.htm 

Todo:
* mv
* du
* file
* find
* wc: https://www.fosslinux.com/45753/linux-wc-command-examples.htm

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

Se quiz 3 i Google forms. Tar upp ungefär följande:

* Hur kan du sortera en lista?
* Hur sparar du den sorterade listan?
* Hur sorterar du på efternamn?
* Hur kan du vända sorteringen?
* Hur kan du slå ihop och sortera namnen från både contacts.txt och kontakter.txt
* Hur kan du söka bland båda listorna?
* Vad gör kommandot: `cat contacts.txt | sort | uniq` ?

### Standard streams: stdin / stdout / stederr

När du skriver ett kommando som tex. `date` syns resultatet i något som heter `stdout`. För en dator är det nästan alltid att visa resultatet på skärmen. Eftersom Unix i många fall används utan skärm (tex en webbserver) vill man kanske att `stdout` ska synas i tex. en loggfil. Det vanliga sättet är använda "redirect operatorn" `>`. Testa i terminalen: `date > datum.txt` och kolla att data landade i filen med `cat datum.txt`.

Inputdata eller `stdin` är för en arbetsdator normalt tangentbordet men med operatorn `<` går det att suga ut data från tex. en textfil. Prova (med exempelfilerna för kontaktlistan): `sort < contacts.txt`.

Läs: https://www.redhat.com/sysadmin/redirect-operators-bash och för att fördjupa kunskaperna: https://www.howtogeek.com/435903/what-are-stdin-stdout-and-stderr-on-linux/

## Loggfiler

Todo:
* tail
* head

## Brew

Vanligaste pakethanteringssystemet (dvs. verktyg för att installera program) för MacOS. Se: https://brew.sh

## Rättigheter (i filsystemet)

Bra men svår guide om rättigheter: https://help.ubuntu.com/community/FilePermissions

Todo:
* filrättigheter (ls -l / chmod)
* användare - grupper (chown / chgrp)
* root - sudo 

## Shell-scripts

https://www.shellscript.sh/

# Trams :)

```
$ say "Hello world!"
$ banner "Hello world!"
```
