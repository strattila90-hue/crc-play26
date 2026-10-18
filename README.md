# CRC PLAY

Mobilra és asztali böngészőre készült, telepíthető, egyoldalas Canvas-játék. A körök célja a feszültség csökkentése, a biztonság és a békés párbeszéd támogatása.

## Indítás

A legegyszerűbb helyben egy statikus webszerverrel futtatni:

```bash
npx serve .
```

Ezután nyisd meg a webszerver által jelzett címet. A telepíthető PWA és az offline gyorsítótár HTTPS-en vagy localhoston működik.

## Irányítás

- `←` / `→` vagy `A` / `D`: mozgás
- `1`, `2`, `3`: vonal, ék, doboz alakzat
- `Szóköz`: párbeszéd vagy békés jelszó
- Mobilon: érintőgombok a játéktér alatt

Válassz szerepet a főmenüben. A kör 90 másodpercig tart; a közelben végrehajtott békés akció csökkenti a feszültséget és pontot ad. A legjobb eredmény eszközönként, helyben mentődik.

## Fájlok

```text
index.html
manifest.webmanifest
sw.js
vercel.json
firebase-config.js
firestore.rules
icons/
images/
```

The same detailed Hungarian CRC soldier is used in the game, main-menu logo and PWA icons. `images/soldier-crc.png` is the transparent game sprite and `images/soldier-crc-source.png` preserves the provided original image.

## GitHub feltöltés

Használd a `CRC-PLAY-GitHub.zip` csomagot: csomagold ki, majd töltsd fel a benne lévő fájlokat és mappákat úgy, hogy az `index.html` közvetlenül a repó gyökerében legyen. Ne töltsd fel a ZIP-et becsomagolva a repóba. Vercelen statikus projektként importáld; build parancs nem kell, a kimeneti mappa a repó gyökere.

## Vercel

Importáld a repót statikus projektként. Build parancs nem szükséges; a projekt gyökere legyen a fenti fájlokat tartalmazó mappa.

## Firebase

A `firebase-config.js` jelenleg helyőrző értékeket tartalmaz. Ranglista bekötése előtt töltsd ki saját Firebase konfigurációval, és ellenőrizd a Firestore szabályokat. A mostani játék a rekordot helyben menti; online ranglista még nincs bekötve.
