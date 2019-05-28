# Sectie de votare:

Fie o sala de votare cu 2 urne, una pentru referendum, iar cealalta pentru Europarlamentare. La intrarea in sala, buletinul persoanei va fi verificat, iar pe baza rezultatului verificarii persoana va fi fie primita sa voteze, fie respinsa. Nu pot fi verificate mai multe persoane in acelasi timp. In sala pot fi prezenti maxim 7 votanti. In sala sunt prezente 5 stampile de vot si 5 cabine de vot. Persoana admisa in sala poate vota pentru referendum, Europarlamentare sau pentru amandoua, lasandu-si cartea de identitate, urmand sa o ia ulterior, dupa ce va termina procesul de votare. Dupa ce alege pentru ce va vota, daca are stampile si cabine disponibile (nu sunt utilizate de alti oameni), acesta va intra intr-o cabina de proba (nu pot intra mai multi oameni intr-o singura cabina). Dupa ce voteaza, individul va plasa in urna, respectiv urnele pentru care si-a ales sa voteze (de exemplu daca o persoana si-a ales sa voteze doar pentru Europarlamentare, aceasta va plasa buletinul de vot in urna pentru Europarlamentare), apoi va putea sa-si ia buletinul inapoi, lucru pe care il si face cand paraseste sala.

Se va contoriza numarul de persoane respinse/nr. de persoane care au votat.

# Cerinta:

Sa se modeleze un sistem, utilizand Tina. Sistemul trebuie sa aiba minim 10 tranzitii. Sa se realizeze analiza sistemului (invarianti, proprietati care se pot deduce pe baza invariantilor, daca este cazul, proprietati generale utilizand graful de accesibilitate/acoperire).

# Reteaua Petri realizata:

![petri_net](https://raw.githubusercontent.com/ac999/laughing-potato/master/img/sdv.png)

# Analiza sistemului:

Pentru analiza mai rapida, vom presupune ca sunt doar 5 oameni care vor sa intre in sala.

![petri_net_a](https://raw.githubusercontent.com/ac999/laughing-potato/master/img/sdva.png)

![arbore_acoperire](https://raw.githubusercontent.com/ac999/laughing-potato/master/img/coverability.png)

De pe analiza arborelui de acoperire putem deduce ca reteaua este finita, ca nu este viabila, dar nu putem spune nimic de reversibilitatea acesteia, in schimb, de pe baza grafului de accesibilitate nu putem deduce viabilitatea retelei:

![graf_accesibilitate](https://raw.githubusercontent.com/ac999/laughing-potato/master/img/marking.png)

Analiza structurala este facuta pe baza retelei cu numar nelimitat de oameni care vor sa intre in sala si este incluse in fisierul [analiza_structurala](./sectie-de-votare-struct.txt)

