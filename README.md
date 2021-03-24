# tesi_pedrinazzi

Nova Fixed key - 11 controlli

Cloud Security Dependencies - 11 controlli

Guest Passwd control 1 - 1 controllo

Guest Passwd control 2 - 7 controlli -----> totale 8

Central directory - 9 controlli

Time sync - 7 controlli


### Mapping dei valori - esempio Nova Fixed key
a0 = 0 ==> valore minimo risultante dai controlli
a1 = 110 ==> valore massimo risultante dai controlli

b0 = 0 ==> valore minimo per membership fuzzy
b1 = 100  ==> valore max per membership fuzzy

a = 110 ==> punteggio risultante

b = b0 + (b1 - b0) ((a - a0)/(a1 - a0))
b = 0 + (100 - 0) ((110 - 0) / (110 - 0))
b = 100 * (110/110)
b = 100 * 1
b = 100 ==> valore risultante dal mapping

