# Kasper til Klean

En personlig landingpage til ansøgningen som AI forretningskonsulent hos Klean. Siden er bygget på koden fra hey-kasper.dk (via ansøgningssiden til Maki) med ny tekst, Kleans grønne farver og Kleans logo.

## Mappen

- site/: selve hjemmesiden. Det er kun denne mappe, der kommer online.
  - index.html: forsiden med al teksten
  - cv.html og ansoegning.html: CV'et og ansøgningen bygget op som PDF'erne i assets/pdf/. Ret teksten begge steder.
  - css/dokument.css: designet til CV og ansøgning (Figtree og farverne fra PDF'erne)
  - en/: de engelske udgaver (index.html, cv.html og application.html). Sprogvælgeren DA/EN i toppen skifter mellem dem. Ret teksten på begge sprog, når noget ændres.
  - 404.html: siden, der vises, hvis adressen er forkert
  - css/styles.css: farver og design. Kleans farver står øverst under `:root`.
  - js/main.js: små forbedringer, fx agentvælgeren i toppen og temaknappen
  - assets/klean-logo.svg: Kleans logo i grøn (#004225)
  - assets/og-image.jpg og og-image-en.jpg: billedet, der vises, når linket deles på LinkedIn eller i en mail
- netlify.toml: fortæller Netlify, at site/ skal publiceres.

## Linket

Siden ligger på GitHub Pages: https://kasperai-stack.github.io/Klean/

Den bliver opdateret automatisk, hver gang der pushes til main (se .github/workflows/pages.yml).

## Se siden på din egen computer

1. Åbn en terminal i mappen.
2. Skriv `npx serve site` og åbn adressen, der vises i terminalen.

## Godt at vide

- Siden skal ikke kunne findes på Google. Den har `noindex` i HTML'en, i netlify.toml og i robots.txt.
- Der er ingen Google Tag Manager, cookies eller formular på siden. Kontakt sker via "Kald til samtale" (mail til kasmussen80@gmail.com) og telefon.
- PDF'erne findes kun på dansk, også når man henter dem fra de engelske sider.
- Teksten følger Kaspers stemme: dansk, "I" og "jer" til Klean, ingen tankestreger og ingen opdigtede tal.
