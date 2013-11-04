Laboratorium 3



1\. Wyświetl plik /etc/passwd z podziałem na strony przyjmując, że strona na 5 linii tekstu. (raczej more niż less).
```
cat /etc/passwd | more -5-p-d
```
2\. Korzystając z polecenia cat utwórz plik tekst3.txt, który będzie składał się z zawartości pliku tekst1.txt, ciągu znaków podanego ze standardowego wejścia (klawiatury) i pliku tekst2.txt.
```
cat >tekst3
cat tekst1 tekst2 >>tekst3
```
3\.Wyświetl po 5 pierwszych linii wszystkich plików w swoim katalogu domowym w taki sposób, aby nie były wyświetlane ich nazwy.
```
head -n5 (sciezka) -q
```
4\.Wyświetl linie o numerach 3, 4 i 5 z pliku /etc/passwd.
```
head -n5 /etc/passwd | tail -n3
```
5\. Wyświetl linie o numerach 7, 6 i 5 od końca pliku /etc/passwd.
```
tail -n 7 /etc/passwd | head -n 3 
```
6\.Wyświetl zawartość pliku /etc/passwd w jednej linii.
```
cat /etc/passwd |tr "\n" " "
```
7\.Za pomocą filtru tr wykonaj modyfikację pliku plik.txt, polegającą na umieszczeniu każdego słowa w osobnej linii.


8\. Zlicz wszystkie pliki znajdujące się w katalogu /etc i jego podkatalogach.
```
ls -a /etc | wc -l
```
9\. Napisać polecenie zliczające ilość znaków z pierwszych trzech linii pliku /etc/passwd.
```
head -n 3 /etc/passwd | wc -c

```
