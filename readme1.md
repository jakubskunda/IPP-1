Implementacni dokumentace k 1 uloze do IPP 2021/2022 \
Jmeno a prijmeni: Jakub Skunda \
login: xskund02 \
<br />

## skript parse.php
vstup : IPPcode22 \
vystup : xml struktura
<br />

### spracovanie argumentov
Argumenty su kvoli rozsireniu STATP spracovavane v cykle, v ktorom je kazda skupina ulozena \
do pola a nasledne sa do tohto pola pridava pole argumentov. 

### spracovanie vstupneho suboru
Subor je spracovavany po riadkoch, v kazdom riadku sa najprv hlada znak #, ak je hladanie uspesne \
nahradi sa on a vsetko za nim prazdnym retazcom. Nasledne sa hlada hlavicka suboru, pretoze musi \
byt na zaciatku, a ak sa najde tak pomocou switch casu sa zacne kontrolovat spravnost instrukcii.

### vytvaranie vystupneho xml suboru
V programe sa najprv inicializuje trieda XMLWriter a zapise sa hlavicka XML, a nasledne sa postupne \
zapisuju do suboru dane instrukcie.



