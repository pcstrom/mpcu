# mpcu-nettside — prosjektoversikt

Dette repoet inneholder to separate nettsider for Per Christian Strøm, begge hostet via GitHub Pages fra repoet `pcstrom/mpcu`.

---

## 1. mpcu.no — matematikkundervisning

**Mappe:** `./` (rotmappen)  
**Fil:** `index.html` + `takk.html`  
**Domene:** mpcu.no (registrert hos Domenshop, DNS peker til GitHub Pages)

### Om siden
Nettside for Per Christians privatundervisningsvirksomhet i matematikk. Målgruppen er elever på videregående som søker ekstraundervisning.

**Bedrift:** Strøm Epitecphro, org.nr. 928 973 042

### Innhold
- Presentasjon av Per Christian som lærer
- Priser og pakker
- Bestill time-lenke (Microsoft Outlook Bookwithme)
- Superprof-annonse
- Personvernerklæring (SharePoint-lenke i footer)

### Design
- Varm, mørk fargepalett: `--dark: #2e2820`, `--accent: #9b7148`, `--bg: #f4efe9`
- Georgia serif for brødtekst, sans-serif for etiketter og knapper
- Ryddig, tillitsvekkende — ikke flashy
- Ingen JavaScript, ingen rammeverk — ren HTML/CSS

### Filer
- `index.html` — hovedside
- `takk.html` — takkeside etter bestilling
- `logo1.png` — logo
- `profilbilde1.jpeg` — profilbilde

---

## 2. Halv Mater — forlag

**Mappe:** `./halvmater/`  
**Fil:** `halvmater/index.html` + forfattersider  
**Domene:** ikke eget domene ennå — publiseres som undermappe av mpcu-repoet

### Om siden
Nettside for forlaget Halv Mater. Siden presenterer utgivelser og forfattere. Inspirasjonsreferanse: Fitzcarraldo Editions (fitzcarraldoeditions.com) — minimalistisk, litterær estetikk.

### Innhold
- Forsiden viser gjeldende utgivelse (Basaliteter av Kjetil Grunnvoll)
- Bestillingsmodul med Vipps og e-post (utsyn@mpcu.no, Vipps 99031130)
- Forfatterliste med lenker til individuelle forfattersider

### Forfattere (midlertidige/fiktive)
- **Kjetil Grunnvoll** — poet, romanforfatter, historiske romaner
- **Prins Eric Hamtørst** — poet, surrealist
- **Elvira Madiganske** — romanforfatter, science fiction

### Design
- Lys, varm bakgrunn: `--bg: #faf9f6`, `--text: #1c1c1a`
- Georgia serif, minimalistisk layout, maks 660px bredde
- Ingen JavaScript, ingen rammeverk — ren HTML/CSS
- Logo: `halvmater/logo.png` (høyde 120px i header)

### Filstruktur
```
halvmater/
  index.html
  logo.png
  basaliteter.jpg        ← bokbilde (midlertidig)
  forfattere/
    kjetil-grunnvoll.html
    prins-eric-hamtorst.html
    elvira-madiganske.html
```

### Viktig: plassering av filer
Alle filer som skal brukes på nettsiden **må ligge i `halvmater/`-mappen** (eller undermapper her). Mappen `mpcu-forlag/` på skrivebordet er et lokalt arbeidsarkiv — filer der er ikke del av repoet og publiseres ikke.

---

## Git og publisering

- **Repo:** `git@github.com:pcstrom/mpcu.git`
- **Branch:** `main`
- **Hosting:** GitHub Pages
- Etter endringer: `git add`, `git commit`, `git push origin main`
- `.DS_Store`-filer skal ikke committes

## Arbeidsform
- Per Christian godkjenner endringer før push til GitHub
- Ren HTML/CSS — ingen rammeverk, ingen build-steg
- Norsk språk i all tekst på sidene
