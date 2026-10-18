# CRC PLAY

Mobilon és asztali böngészőben futó, Canvas-alapú, telepíthető PWA. A játék a kommunikációra, a civilbiztonságra és a nyugodt helyzetkezelési döntésekre összpontosít. A felhasználói katonaillusztráció szerepel a játékban, a menüben és az alkalmazásikonokon.

## GitHub feltöltés

1. Csomagold ki a `CRC-PLAY-GitHub.zip` fájlt.
2. Töltsd fel a benne lévő fájlokat és mappákat a GitHub-repó gyökerébe. Az `index.html` közvetlenül a gyökérben legyen.
3. Vercelen válaszd az `Other` / statikus projektet. Build parancs nem szükséges, a kimeneti mappa `.`.

## Helyi indítás

HTTPS-en vagy localhoston futtasd. Egyszerű statikus szerverrel: `npx serve .`.

## Fő fájlok

- `index.html` – a teljes játék, külső build nélkül
- `manifest.webmanifest`, `sw.js` – telepíthető PWA és offline gyorsítótár
- `images/soldier-crc.png` – átlátszó hátterű játékbeli katona
- `images/soldier-crc-source.png` – az eredeti forrásillusztráció
- `icons/` – Android, maskable és Apple ikonok
- `vercel.json` – statikus Vercel útvonalkezelés

A Firebase-fájlok helyőrző konfigurációt tartalmaznak; online ranglista nincs bekötve. A rekordok helyben, böngészőnként mentődnek.
