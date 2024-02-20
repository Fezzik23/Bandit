## Bandit 0
```bash
ssh -p 2220 bandit0@bandit.labs.overthewire.org
bandit0
cat readme
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
```
## Bandit 1
```bash
ssh -p 2220 bandit1@bandit.labs.overthewire.org
bandit1@bandit.labs.overthewire.org
cat /home/bandit1/-
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi
```
## Bandit 2
```bash
ssh -p 2220 bandit2@bandit.labs.overthewire.org
cat spaces\ in\ this\ filename
aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
```
## Bandit 3
The password for the next level is stored in a hidden file in the inhere directory.
```bash
ssh -p 2220 bandit3@bandit.labs.overthewire.org
ls -apls
cat .hidden
2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
```
## Bandit 4
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.
```bash
ssh -p 2220 bandit4@bandit.labs.overthewire.org
cat ./-file07 
(./ para evitar que lo interprete como comando)
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
```
## Bandit 5
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:
human-readable
1033 bytes in size
not executable
```bash
ssh -p 2220 bandit5@bandit.labs.overthewire.org
find . -size 1033c
./maybehere07/.file2
cat ./maybehere07/.file2
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
```
## Bandit 6
The password for the next level is stored somewhere on the server and has all of the following properties:
owned by user bandit7
owned by group bandit6
33 bytes in size
```bash
ssh -p 2220 bandit6@bandit.labs.overthewire.org
find . -size 33c -user bandit7 -group bandit6
./var/lib/dpkg/info/bandit7.password
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
```

## Bandit 7
The password for the next level is stored in the file data.txt next to the word millionth
```bash
ssh -p 2220 bandit7@bandit.labs.overthewire.org
grep -e millionth data.txt
TESKZC0XvTetK0S9xNwm25STk5iWrBvP
```

## Bandit 8
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once
```bash
ssh -p 2220 bandit8@bandit.labs.overthewire.org
sort data.txt | uniq --unique
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
```

## Bandit 9
The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.
```bash
ssh -p 2220 bandit9@bandit.labs.overthewire.org
(es que he hecho un cat del fichero y me ha salido la pwd en la cara)
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
```
## Bandit 10
The password for the next level is stored in the file data.txt, which contains base64 encoded data
```bash
ssh -p 2220 bandit10@bandit.labs.overthewire.org
```