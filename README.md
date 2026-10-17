# Halden — sajt studija za arhitekturu

Statičan sajt na jednoj stranici, tamna tema, srpski i engleski. Ne treba mu server ni build: radi direktno na GitHub Pages.

## Sadržaj

| Fajl | Šta je |
|---|---|
| `index.html` | Ceo sajt (kod, fontovi i slika iz hero sekcije su spakovani u jedan fajl) |
| `assets/` | Fotografije projekata i faza rada |
| `config.js` | Podešavanja: e-pošta studija i slanje upita |
| `404.html` | Stranica za nepostojeće adrese |
| `.nojekyll` | Kaže GitHub Pages-u da fajlove servira takve kakvi su |

## Objavljivanje na GitHub Pages

1. Na GitHub-u napravi novi repozitorijum (npr. `halden-website`).
2. Otpremi **sadržaj** ovog foldera (ne sam folder): `index.html`, `config.js`, `404.html`, `.nojekyll` i ceo `assets/` folder.
   Najlakše: **Add file → Upload files**, prevuci sve fajlove i folder `assets`, pa **Commit changes**.
   Napomena: `.nojekyll` je skriven fajl na nekim sistemima; ako ga ne vidiš, sajt radi i bez njega.
3. **Settings → Pages → Build and deployment**: Source **Deploy from a branch**, Branch **main**, folder **/ (root)**, pa **Save**.
4. Posle minut-dva sajt je na `https://<korisničko-ime>.github.io/halden-website/`.

## Forma za upit

Bez podešavanja forma otvara program za e-poštu posetioca sa već popunjenim upitom.

Da upiti stižu direktno na tvoju e-poštu, bez programa za poštu:
1. Napravi besplatan nalog na [formspree.io](https://formspree.io) i novu formu.
2. Kopiraj adresu forme (izgleda kao `https://formspree.io/f/abcdwxyz`).
3. U `config.js` upiši je u `formEndpoint`, a pravu adresu studija u `email`.

## Pre objave proveri

- E-pošta `studio@halden.archi` je primer: upiši pravu u `config.js`.
- Linkovi Instagram / LinkedIn / Are.na u futeru još ne vode nigde (`#`).
- Trajanja faza u sekciji „Kako radimo“ su predlog: uskladi ih sa stvarnim radom studija.
- Fotografije su sa Unsplash-a (besplatna licenca, dozvoljena i komercijalna upotreba).

## Lokalni pregled

Otvori `index.html` dvoklikom. 3D model učitava biblioteku three.js sa interneta, pa je za njega potrebna veza.
