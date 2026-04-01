# Summary — dhobalova.cz

## Stav projektu
**Datum:** 2026-04-01
**Status:** Dokončeno — web vytvořen, GitHub push probíhá

---

## Co bylo vytvořeno

Jednostránkový moderní web pro **Dentální hygienu Alena Obalová, DiS.** v Uherském Hradišti.

### Technologie
- Čistý HTML5 + CSS3 + vanilla JS (single file `index.html`)
- Google Fonts: **Syne** (nadpisy) + **Nunito** (tělo) — v portfoliu dosud nepoužito
- Intersection Observer pro fade-up animace
- Hamburger menu pro mobil
- Google Maps iframe embed

### Barevná paleta (unikátní v portfoliu)
| Proměnná | Hex | Role |
|----------|-----|------|
| `--bg` | `#FAFCFF` | Hlavní pozadí |
| `--surface` | `#F0F4FF` | Alternativní sekce |
| `--indigo` | `#4F46E5` | Primární akcent — buttons, ikony |
| `--indigo-dark` | `#3730A3` | Hover stav |
| `--mint` | `#10B981` | Sekundární akcent — hero badge, CTA |
| `--dark` | `#111827` | Tmavé sekce, footer |

### Sekce (v pořadí)
1. **Nav** — sticky, transparent→bílá, hamburger
2. **Hero** — gradient indigo→blue, split layout (text + glassmorphism karta)
3. **O nás** — split grid, barevná karta s AO avatarem + float karty
4. **Pojišťovny** — insurance strip (VZP, VoZP, ČPZP, OZP, ZPMVČR, MV ČR)
5. **Služby** — 3×2 grid karet s cenami (6 služeb)
6. **Postup** — 4 kroky jak návštěva probíhá
7. **Ordinační doba** — tabulka hodin + CTA box
8. **Kontakt** — kontaktní info + formulář
9. **Mapa** — Google Maps iframe
10. **Footer** — 3 sloupce + copyright

### Responzivita
- 960px: gridy přechází na 2 sloupce
- 640px: vše na 1 sloupec, hamburger menu
- 428px / 375px / 320px: menší fonty, padding

### Reálné informace ze scrapu dhobalova.cz
- **Provozovatelka:** Alena Obalová, DiS.
- **Telefon:** +420 731 657 079
- **Email:** obalova.alca@seznam.cz
- **Adresa:** Dlouhá 228, Dům HUBERT, Uherské Hradiště
- **Ceny:** Vstupní 1 350 Kč, Recall od 950 Kč, Dom. bělení 5 800 Kč, Ord. bělení 6 000 Kč
- **Ordinace:** Po 7:30–15, Út 7:30–18, St 7:30–13, Čt 7:30–15, Pá 7:30–13

---

## Vizuální odlišení od DNA portfolia
- **Jiné od Rehabilitace UH** (tam navy/teal, Raleway+Source Sans) — zde vivid indigo + emerald mint, Syne+Nunito
- **Jiné od Centrum Zdraví** (sage/forest, Cormorant+Jost) — zcela jiná paleta a typografie
- **Jiné od Kosmetiky** (blush/rose, Playfair+DM Sans) — žádné teplé růžové tóny
- **Jiné od Machaly** (burnt orange, Space Grotesk+Figtree) — studená, čistá paleta

## GitHub
- Repo: https://github.com/supercigan/dhobalova
- Vercel: auto-deploy z master branch
