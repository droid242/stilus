# stilus
Stílus gyakorlás

CSS Box Model - hajtogassunk dobozt
Az úgynevezett doboz modell azt mutatja meg, hogyan épülnek fel az elemek, és hogyan helyezkednek el egymáshoz képest a böngészőben.


Margin
Kívülről befelé haladva az első eleme a box-modelnek a margin. Ez nem része konkrétan az elemnek, ez az elhagyás az elem körül. Magyarul margónak is nevezhetjük. A legtöbb elem rendelkezik alapértelmezett marginnal, ezt tudjuk a saját CSS szabályainkkal felülbírálni.

Meg lehet adni oldalanként vagy egy utasítással is:
oldalankénti megadás: margin-top, margin-right, margin-bottom, margin-left
megadás egyben: margin: top right bottom left
megadás páronként: margin: top-bottom right-left


Border
A következő a border, vagy szegély. Ha nem adjuk meg, akkor a vastagsága 0px lesz. Az elem méretét növeli a border vastagsága, azaz ha 2px a border, akkor az elem minden irányban 4 pixellel szélesebb lesz.

Megadása:
egy utasítással: border: style width color;
sarkak kerekítése: border-radius: 10px;
oldalanként: border-left: style width color;
tulajdonságonként: border-style, border-width, border-color


Padding
Itt már az elemen belül járunk, úgy is mondhatnám, hogy átléptük a határt (border). Tehát ez már az elem belső padkája, az elemen belül ennyivel beljebb kezdődik a tartalom. Az elem méretét akkor növeli, ha a box-sizing: border-box; nincs beállítva.

***

Box-shadow
A box-shadow az elemet körülvevő vetett árnyék. A CSS3 hozta be. Az alábbi séma szerint lehet megadni, amit a videóban részletesen elmagyarázok:

box-shadow: none|h-shadow v-shadow blur spread color|inset|initial|inherit;

***

%, em, rem
%: a méretet a befogadó elem méretének százalékában adja meg.
em: a betűméret, 1 esetén megegyezik, de például az 1.5 másfélszeres.
rem: root em, nem a szülő elem em-jét nézi, hanem a <html> elemét.