Laboratorium 1

1\. Używając linii poleceń stwórz strukturę katalogów:

```sh
mkdir -p nauka/{c,logo,pascal} dom praca/{dokumenty,zlecenia/{niezrealizowane,zrealizowane}}
```

2\. Przejdź do katalogu dom i utwórz katalog wazne-sprawy.:

```sh
cd dom
mkdir wazne-sprawy
```

3\. Wejdź do katalogu wazne-sprawy i utwórz tam pusty plik rachunki.txt.

```sh
cd dom
cd wazne-sprawy
touch rachunki.txt
```

4\. Będąc w katalogu wazne-sprawy skopiuj plik rachunki.txt do katalogu zrealizowane.

```sh
cp rachunki.txt ../../praca/zlecenia/zrealizowane
```

5\. Przejdź do katalogu zrealizowane i zmień nazwę pliku rachunki.txt na wykonano.txt.

```sh
cd praca
cd zlecenia
cd zrealizowane
mv rachunki.txt wykonano.txt
```

6\. Utwórz plik wykonano.txt wielkości 11 bajtów, następnie podziel go pliki wielkości 5 bajtów.
W ten sposób otrzymasz 3 pliki. (split)

```sh
echo 1234567890 > wykonano.txt
split --bytes=5 wykonano.txt
```

7\. Będąc w katalogu logo skopiuj powyżej otrzymane 3 pliki do katalogu dokumenty.

```sh
cd nauka
cd logo
cp ../../praca/zlecenia/zrealizowane/xaa xab xac ../../praca/dokumenty
```

8\. Będąc w katalogu dokumenty połącz skopiowane 3 pliki w plik odtworzono.txt, tak aby otrzymać plik o zawartości
identycznej z wykonano.txt. Następnie plik odtworzono.txt skopiuj do katalogu wazne-sprawy.

```sh
cd praca
cd dokumenty
cat x* >> odtworzono.txt
cp odtworzono.txt ../../dom/wazne-sprawy
```

9\. Będąc w katalogu wazne-sprawy sprawdź, czy są jakieś różnice w zawartości plików wykonano.txt i odtworzono.txt.

```sh
diff odtworzono.txt ../../praca/zlecenia/zrealizowane/wykonano.txt
```

10\. Wyświetl kalendarz na październik 2009 r. (cal)

```sh
cal 10 2009

cal 10 2009 -3
```

11\. Jaki był dzień tygodnia 25 maja 1975 r.

```sh
date -d 1975-05-25 +%A
```
