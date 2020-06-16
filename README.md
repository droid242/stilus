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

***

Display vs. visibility
display
A display tulajdonság az elem megjelenítését befolyásolja. Azt mondja meg, hogy a böngészőnek figyelembe kell-e vennie az elemet az oldal megjelenítésekor, és ha igen, akkor hogyan.

Használata: display: inline|block|flex|inline-block|none;
block: nincs mellette más elem
inline: mindig egysorban
none: nem jelenik meg

A none érték azt írja elő, hogy nem kell megjeleníteni az elemet. A megjelenített oldalon a böngésző nem foglal helyet az elemnek, ezért a felhasználó nem láthatónak érzékeli.

visibility
Ezzel szemben a visibility csak a láthatóságot módosítja. Tehát ha elrejtjük vele az elemet, akkor a helyfoglalás megmarad.

Használata: visibility: visible|hidden|collapse|initial|inherit;
hidden: elrejtve

***

Position - helyezkedjünk kicsit!
Azt adhatjuk meg vele, hogyan legyen kalkulálva az elem pozíciója.

position: static; ez az alapértelmezett, a helyzet a többi elemtől függ.
position: relative; a helyzet a saját normál pozíciótól függ.
position: fixed; a böngészőablakhoz képest helyezkedik el.
position: absolute; a helyzet az első nem static elemtől függ.