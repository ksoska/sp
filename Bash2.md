Laboratorium 2

1\. Wyświetl na ekran 2 pierwsze wiersze pliku program.c. (head)
```sh
head -2 program.c
```
2\. Wyświetl na ekran 4 ostatnie wiersze pliku program.c. (head, tail)
```sh
tail -4 program.c
```
3\.W pliku program.c znajdź wszystkie wiersze z wystąpieniem słowa „main”. (grep)
```sh
cat program.c | grep main
```
4\.Plikowi program.c nadaj następujące uprawnienia: właściciel – czytanie, pisanie, grupa – czytanie, pozostali użytkownicy: brak uprawnień. (chmod)
```sh
chmod 640 program.c
```
5\.Będąc w katalogu temp przenieś katalog wazne-sprawy do katalogu praca.
```sh
cd temp
mv dom/wazne-sprawy praca
```
6\. Zarchiwizuj cały katalog temp. (zip i tar)
```sh
tar -czf temp.tar.gz temp;
```
7\. Usuń katalog temp.
```sh
rm temp -r
```
8\. Odtwórz z archiwum katalog temp. (unzip i tar)
```sh
tar -xzf temp.tar.gz
```
9\. Posprzątaj na swoim koncie.
```sh
rm temp* -r
```
10\. Wyswietl linijki ze srodka programu (liczac od gory). Przyklad : pokaz linijki 3 i 4.

```sh
head -n4 program.c | tail -n2
```
11\. Wyswietl linijki ze srodka programu (liczac od dolu). Przyklad : pokaz linijki 5 i 6.
```sh
tail -n6 program.c | head -n2
```
