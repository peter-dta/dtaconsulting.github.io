# DTA Consulting – umbrella weboldal

Statikus, függőségmentes (HTML + CSS + egy kis JS) magyar nyelvű oldal.

## Futtatás helyben

```
cd dta-consulting
python3 -m http.server 8080
```

Majd: http://localhost:8080

## Fájlok

- `index.html` – teljes tartalom, metaadatok, Open Graph
- `styles.css` – design (színek a `:root` változókban)
- `adatkezelesi-tajekoztato.html` – adatkezelési tájékoztató (a jóváhagyott, kitöltött Word-változat alapján)
- `script.js` – mobilmenü, fejléc-árnyék, dinamikus évszám
- `assets/` – vektoros (SVG) logókészlet: világos/sötét/fekete/fehér, álló és vízszintes változat, jel (ikon) és kerek emblémaikon; `apple-touch-icon.png` az emblémából

## Hiányzó / cserélendő

- Logók: az SVG-k a lookbook képéről lettek újraépítve (a D, T, A jel mért geometriából, a CONSULTING felirat Montserrat Regular körvonalakból), nem az eredeti tervezői fájlból. Ha lesz eredeti vektoros fájl, cserélendők. A kerek emblémaikon gyűrűjének apró ívei közelítések.
- Formspree: az űrlap az `xeaenrgd` azonosítójú formra küld (`index.html`, `action`). A Formspree-ben érdemes a domain-korlátozást beállítani, és az első levél megerősítését jóváhagyni.
- Open Graph kép (`og:image`) – nincs.
- A `dtax.hu` és a `kapcsolodascoaching.hu` élesedett: a márkakártyákon és a láblécben linkelve vannak.
- A márkák kiemelő színei (`--accent` az `index.html`-ben) csak javaslatok, nem hivatalos márkaszínek.

## Kézi ellenőrzést igényel

- A székhely a régi dta-consulting.hu oldalról származik. Telefonszám szándékosan nincs kint.
- A kapcsolodascoaching.hu és a sechack.hu nem volt automatikusan olvasható; a leírások a megadott szövegek.
- A canonical / og:url (`https://dta-consulting.hu/`) feltételezett végleges cím.
- Betűtípus: rendszer-/Montserrat-verem, külső betöltés nélkül. Ha a Montserrat kell mindenkinek, érdemes saját hosztolni.

## Adatkezelési tájékoztató

Az `adatkezelesi-tajekoztato.html` a jóváhagyott, kitöltött Word-változat szövegét tartalmazza (adatkezelő adatai, GitHub Pages tárhely, Formspree, 12 hónapos megőrzés).
- A tájékoztató azt állítja, hogy az oldal nem használ sütit/analitikát, és nem tölt be külső tartalmat. Ez a jelenlegi kódra igaz; új szolgáltatás (pl. analitika, külső betűtípus, térkép) beépítésekor a tájékoztatót is frissíteni kell.
- A tájékoztató a GitHub Pages tárhelyet nevezi meg. Ha az oldal más tárhelyre költözik, a 2.2., 4. és 5. szakaszt módosítani kell.
- A szöveg változtatásakor frissítsd a „Utolsó frissítés” dátumot is.
