Implementační dokumentace k 1. úloze do IPP 2021/2022 \
Jméno a příjmení: Jakub Škunda \
Login: xskund02 \
<br />

## skript parse.php
Vstup : IPPcode22 \
Výstup : xml struktura
<br />

### Spracovanie argumentov
Argumenty sú kvôli rozšíreniu STATP spracovávané v cykle, v ktorom je každá skupina uložená \
do poľa a následne sa do tohto pola pridava pole argumentov. \
Ak je v poli argv na prvom mieste argument --help, tak sa na standardny vystup vypise napoveda. 
<br />

### Spracovanie vstupného súboru
Subor je spracovavany po riadkoch, v kazdom riadku sa najprv hlada znak #, ak je hladanie uspesne \
nahradi sa on a vsetko za nim prazdnym retazcom. Nasledne sa hlada hlavicka suboru, pretoze musi \
byt na zaciatku, a ak sa najde tak sa pomocou switch case zacne kontrolovat spravnost instrukcii. \
Instruckie su rozdelene do skupin podla typu vstupnych argumentov. 
<br />

#### funkcia checksymb 
Funkcia kontroluje spravnost argumentov pomocou regexov, a vracia typ symbolu (pripadne oznacenie premennej) \
a jeho hodnotu (pri premennej nazov).
<br />

### vytvaranie vystupneho xml suboru
V programe sa najprv inicializuje trieda XMLWriter a zapise sa hlavicka XML, a nasledne sa postupne \
zapisuju na standardny vystup dane instrukcie.
<br />

#### funkcia WriteElement
Funkcia ktorej je predana trieda XMLWriter, nazov instrukcie a pripadne jej argumenty. Tato funkcia nasledne \
vykonava zapis na standartny vystup.
<br />

### Implementovane rozsirenia
<br />

#### STATP
Pre jednotlive parametre som vytvoril premenne, ktore postupne za behu programu inkrementujem, a na konci \
programu podla toho ci su ziadane alebo nie vypisem do vystupneho suboru. \
<br />

#### NVP
Ako triedu som pouzil uz spominany XMLWriter. Pre pracu s nim som pouzil oficialnu dokumentaciu  

"""
ahoj
"""
