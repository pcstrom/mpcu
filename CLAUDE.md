# mpcu-nettside — prosjektoversikt

Dette repoet inneholder nettsiden for Per Christians matematikkundervisningsvirksomhet, hostet via GitHub Pages på domenet **mpcu.no**.

> Halv Mater forlag har egen repo (`pcstrom/halvmater`) og eget domene (**halvmater.no**) — flyttet ut mai 2026. Se `~/Desktop/halvmater-nettside/`.

---

## mpcu.no — matematikkundervisning

**Mappe:** `./` (rotmappen)  
**Filer:** `index.html`, `takk.html`, `salgsvilkar.html`  
**Domene:** mpcu.no (registrert hos Domenshop, DNS peker til GitHub Pages)

### Om siden
Nettside for Per Christians privatundervisningsvirksomhet i matematikk. Målgruppen er elever på videregående og privatister som søker ekstraundervisning.

**Bedrift:** Strøm Epitecphro, org.nr. 928 973 042  
**Adresse:** Marithaugen 24 A, 8310 Kabelvåg  
**E-post:** pc@mpcu.no

### Priser (gjeldende per mai 2026)
| Tjeneste | Pris |
|---|---|
| Avklaringssamtale, inntil 20 min | Gratis |
| Undervisning, 60 min | 750 kr |
| Undervisning, 90 min | 1 100 kr |
| Eksamensrettet intensivøkt, 120 min | 1 450 kr |
| Klippekort 5 × 60 min | 3 600 kr |
| Klippekort 10 × 60 min | 7 000 kr |

Betaling: Vipps-lenke sendes etter gjennomført time. Klippekort faktureres ved oppstart. Ingen mva på undervisning.

### Fag som undervises
1P, 1P-Y, 1T, 2P, 2P-Y, S1, S2, R1, R2, X

### Sidestruktur og seksjoner (index.html)
1. **Nav** — sticky, mørk. Venstre: «Strøm Epitecphro». Høyre: «Bestill time»-knapp.
2. **Hero** — lys varm bakgrunn (`--bg-warm`). Badge med stjernesnitt, h1, ingress, CTA-knapp + profilbilde i rad. Bildet er klikkbart og lenker til bookingsiden.
3. **Stats** — tre tall: 20 år erfaring, 5★ snitt, Lektor & sensor.
4. **Om meg** — sirkulært profilbilde til venstre for tekst.
5. **Undervisning** — beskrivelse av metode + tre feature-kort (Tilpasset deg, Eksamensfokus, Online og interaktivt).
6. **Fag** — taggar for alle matematikkfag.
7. **Priser** — tabell med alle tjenester og priser + mva-note.
8. **Hva undervisningen kan omfatte** — tabell med innholdsbeskrivelser (Kartlegging, Individuell plan, Eksamensstrategi, osv.).
9. **Anmeldelser** — tre sitater fra Superprof.
10. **CTA bunn** — mørk seksjon med bookinglenke.
11. **Footer** — © Strøm Epitecphro, e-post, org.nr., lenke til salgsvilkår, lenke til personvernerklæring.

### Viktige lenker
- **Bookingside:** `https://outlook.office.com/bookwithme/user/791a7a23e38f4585b57d53923348e6c2@mpcu.no?anonymous&ismsaljsauthenabled&ep=plink`
- **Superprof-profil:** `https://www.superprof.no/lektor-sensor-matematikk-ars-erfaring-hjelp-til-eksamen-bedre-karakterer-tryggere-problemlosning.html`
- **Personvernerklæring:** `https://epitecphro-my.sharepoint.com/:b:/g/personal/pc_mpcu_no/IQClG9r6yn2AQ5XDnKpOiYP2Ab1s4b5l6EK20vo4bMeZSHk?e=ac0Pbf`
- **Salgsvilkår:** `mpcu.no/salgsvilkar` — opprettet for Vipps-registrering (behandlingstid inntil én uke per mai 2026)

### Design
- Varm, mørk fargepalett: `--dark: #2e2820`, `--accent: #9b7148`, `--bg: #f4efe9`, `--bg-warm: #ede7df`
- Hero-seksjonen bruker `--bg-warm` (ikke mørk gradient — ble endret fordi den var for dyster)
- Georgia serif for brødtekst, sans-serif for etiketter og knapper
- Google Analytics: `G-BEXQ3YTYLW` — booking-klikk spores med `gtag('event','booking_click',...)`
- Profilbilde: `profilbilde1.jpeg` — brukes i hero (liten sirkel ved siden av knapp) og i Om meg-seksjonen

### Filer
- `index.html` — hovedside
- `takk.html` — takkeside etter bestilling
- `salgsvilkar.html` — salgs- og betalingsvilkår (opprettet mai 2026 for Vipps-registrering)
- `profilbilde1.jpeg` — profilbilde Per Christian

### Designprinsipper og preferanser
- Nøkternt og seriøst uttrykk — ikke flashy
- Per Christians navn brukes i CTA-knapper for å myke opp og personliggjøre («Bestill din første time med Per Christian →»)
- Firmanavnet Strøm Epitecphro brukes i nav og footer for profesjonelt inntrykk
- Neste naturlige steg: logo og eventuelt bedre profilbilde

---

## Git og publisering

- **Repo:** `git@github.com:pcstrom/mpcu.git`
- **Branch:** `main`
- **Hosting:** GitHub Pages
- Etter endringer: `git add`, `git commit`, `git push origin main`
- `.DS_Store`-filer skal ikke committes

## Arbeidsform
- Ren HTML/CSS — ingen rammeverk, ingen build-steg
- Norsk språk i all tekst på sidene
- Per Christian liker nøkternt og seriøst uttrykk — ikke overdesigne
