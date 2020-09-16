# doktorat-dariusza-izaka
Dane do doktoratu pana magistra Dariusza Izaka

Cześć Darek.

Udoskonaliłem Twój software i stworzyłem program, który działa z linii komend.

Wykonanie zadania o które prosiłem było trochę bardziej złożone i wymagało użycia wyrażeń regularnych (Regular Expressions), co jest dość złożoną i abstrakcyjną koncepcją matematyczną informatyczną. Trudno mi jest wyjaśnić to w krótkim opisie. Nie przejmuj się jeśli nie rozumiesz tej części kodu.

Podstawowa gramatyka jest następująca:

python dla_izak.py species_list list_of_genes ll

Gdzie: dla_izak.py kod pythona species_list plik zawierający listę gatunków (nazwy według KEGG) list_of_genes plik z listą genów ll nazwa outputu W wyniku działania programu powstają pliki: ll.tsv i ll.xlsx

Zmieniłem sposób pobierania nazw gatunków i symboli z serwera KEGG. W twojej wersji programu pierwotnie, pobierałeś za pomocą kilku funkcji. Jest to jednak rozwiązanie mało stabilne, bardzo zależne od ustawień serwera KEGG, wersji pythona i tak dalej. Ja stworzyłem plik specie, który zawiera podstawowe dane. Pobierany jest on za pomocą funkcji read_pickle i nie wiem, czy jest to najbardziej uniwersalny sposób zapisywania danych. Może trzeba to zakodować inaczej.
