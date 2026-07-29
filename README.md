# Pohance — demo landing stranica

Jednostranični demo sajt za izmišljenu firmu **Pohance**, koja iznajmljuje napuhance za dječje
rođendane i evente. Dvojezično: **hrvatski / njemački**, s prekidačem u navigaciji.

## Pokretanje

Otvorite `index.html` u pregledniku. Nema build koraka, nema ovisnosti.

## Tehnologije

Čist HTML, CSS i vanilla JavaScript — sve u jednom `index.html` (CSS u `<style>`, JS u `<script>`).
Mobile-first i responzivno, spremno za GitHub Pages.

## Sadržaj

Hero · Zašto mi (4 kartice) · Ponuda (3 napuhanca) · Kako funkcionira (3 koraka) ·
Recenzije · FAQ · Kontakt forma · Footer

## Dvojezičnost

Prekidač **HR / DE** u navigaciji.

- Hrvatski tekstovi žive izravno u HTML-u (`data-i18n="kljuc"`) i pri učitavanju se snimaju u memoriju.
- Njemački prijevodi su u objektu `DE` na vrhu `<script>` bloka.
- Prevode se i atributi: `data-i18n-placeholder`, `data-i18n-aria-label`, `data-i18n-content`.
- Odabir jezika pamti se u `localStorage`; prvi posjet preuzima jezik iz postavki preglednika.

Dodavanje novog teksta: stavite `data-i18n="neki.kljuc"` na element s hrvatskim tekstom i dodajte
isti ključ u objekt `DE`.

## GitHub Pages

Settings → Pages → Source: `main` / root. Stranica je odmah dostupna jer je sve statično.

## Napomena

Demo — sve cijene, recenzije i kontakt podaci su izmišljeni. Forma ne šalje podatke nigdje;
validacija i poruka o uspjehu izvode se lokalno u pregledniku.
