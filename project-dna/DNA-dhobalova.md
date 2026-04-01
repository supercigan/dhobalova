# DNA — dhobalova (Dentální hygiena Alena Obalová)

## Vizuální archetype
**"Clean Precision"** — svěží, moderní zdravotní web. Vivid indigo jako hlavní akcent evokuje profesionalitu a důvěryhodnost. Emeraldová máta přidává pocit čerstvosti a čistoty typický pro dentální péči. Světlé, vzdušné, přehledné — bez agresivity.

## Barevná paleta
| Proměnná | Hex | Role |
|----------|-----|------|
| `--bg` | `#FAFCFF` | Hlavní pozadí (studená bílá) |
| `--surface` | `#F0F4FF` | Alternativní sekce (světle indigo-bílá) |
| `--surface-2` | `#E8F5EF` | Zelenkavé povrchy |
| `--indigo` | `#4F46E5` | Primární akcent — tlačítka, ikony, hero gradient |
| `--indigo-dark` | `#3730A3` | Hover stav indiga |
| `--indigo-light` | `#EEF2FF` | Pozadí ikonových boxů |
| `--mint` | `#10B981` | Sekundární akcent — CTA tlačítko, badge, floats |
| `--mint-dark` | `#059669` | Hover máty |
| `--mint-light` | `#D1FAE5` | Světlé mint pozadí karet |
| `--dark` | `#111827` | Tmavé sekce (hours), footer |
| `--dark-2` | `#1F2937` | Footer bg |
| `--text` | `#374151` | Tělo textu |
| `--muted` | `#6B7280` | Sekundární text |
| `--border` | `#E5E7EB` | Bordery |

**Proč tato paleta:** Vivid indigo + emerald mint — kombinace dosud nepoužitá v portfoliu. Studená, svěží, čistá — odpovídá oboru dentální hygieny. Kontrastuje s teplými paletami (Centrum Zdraví, Kosmetika, Machala) i tmavou navy (Rehabilitace).

## Typografie
| Role | Font | Důvod |
|------|------|-------|
| Nadpisy h1–h4 | **Syne** (700, 800) | Geometrický, architektonický, výrazný — v portfoliu dosud nepoužit |
| Tělo textu | **Nunito** (400, 500, 600, 700) | Přátelský, kulatý, výborně čitelný — pro všechny věkové skupiny |

- Base font-size: 1rem = 16px
- Line-height text: 1.75
- Line-height nadpisy: 1.15

## Layout & Struktura sekcí
```
NAV (fixed sticky, transparent → bílá s blur po scrollu, hamburger)
HERO (min-height 100vh, gradient indigo→blue, split 2 sloupce)
  ├── Vlevo: badge + H1 + subtitle + 2 CTA buttons
  └── Vpravo: glassmorphism karta s info, chips, stats grid
WAVE A (hero → about)
O NÁS (white bg, split grid: vizuální karta AO vlevo, text vpravo)
POJIŠŤOVNY (insurance strip, flex-wrap badges)
WAVE B (about → services, F0F4FF)
SLUŽBY (surface bg, 3×2 grid karet s cenami, top-border hover)
WAVE A (services → process, white)
POSTUP (white bg, 4 kroky v řadě, circular čísla)
WAVE B (process → hours, #111827)
ORDINAČNÍ DOBA (tmavá sekce, tabulka + CTA box s gradientem)
WAVE A (hours → contact, bg)
KONTAKT (bg, split: kontaktní info + formulář)
MAPA (Google Maps iframe, full-width)
FOOTER (dark-2, 3 sloupce: brand / nav / kontakt)
```

## Klíčové designové prvky

### Hero glassmorphism karta
- `backdrop-filter: blur(16px)`, `rgba(255,255,255,0.1)` border
- 2×2 stats grid se zelenými čísly (--mint)
- Chips: AIR FLOW, Bělení zubů, Parodontitida, Děti i dospělí
- Blinking green dot badge "Přijímáme nové pacienty"

### About karta
- Gradient indigo karta s AO avatarem (iniciály)
- Float karty pod: zelená (přijímáme pacienty) + indigo (adresa)

### Service cards
- `::before` pseudo-element top border — scaleX(0→1) při hover (gradient indigo→mint)
- Čísla 01–06 jako service-num tag
- Cena zvýrazněna v indigo barvě (Syne font)

### Process steps
- Circular čísla s indigo border
- Hover: vyplnění indigo + bílé číslo
- Horizontální linka connecting steps (desktop) — `::before` gradient

### Dark hours sekce
- Jediná tmavá sekce (#111827) — výrazný vizuální předěl
- Tabulka hodin s tmavými řádky
- Zelená info box pro poznámku o víkendu
- Gradientní CTA box (indigo)

## Responsivita
| Breakpoint | Změna |
|-----------|-------|
| 960px | Hero jednosloupcový, services 2 sloupce, hours/contact 1 sloupec |
| 640px | Hamburger nav, vše 1 sloupec, hero buttons full-width column |
| 428px | Menší fonty hero/title, menší nav padding |
| 375px | Ještě menší hero-title (2rem) |
| 320px | Minimální velikosti, buttons compact |

## Co se osvědčilo
- Vivid indigo je výrazný, nepůsobí korporátně, perfektní pro zdravotnictví
- Syne font — výrazný, moderní, nezaměnitelný v portfoliu
- Glassmorphism hero karta — elegantní způsob zobrazení info bez přeplnění
- Tmavá hours sekce jako střední vizuální předěl (alternace světlé/tmavé)
- Float karty v About sekci: přirozené, informativní bez grid tuhosti
- Insurance strip — neintruzivní ale viditelná informace o pojišťovnách

## Co příště jinak
- Hero karta mohla mít real fotku hygienistky místo AO avatara
- Google Maps embed může mít nepřesné souřadnice — zkontrolovat při ostrém nasazení
- Formspree nebo jiný backend pro kontaktní formulář (aktuálně jen JS mock)

## Byznys informace
| Položka | Hodnota |
|---------|---------|
| Provozovatelka | Alena Obalová, DiS. |
| Telefon | +420 731 657 079 |
| Email | obalova.alca@seznam.cz |
| Adresa | Dlouhá 228, Dům HUBERT, 686 01 Uherské Hradiště |
| Vstupní návštěva | 1 350 Kč |
| Recall návštěva | od 950 Kč |
| Domácí bělení | 5 800 Kč |
| Ordinační bělení | 6 000 Kč |

**Ordinační hodiny:**
- Po: 7:30 – 15:00
- Út: 7:30 – 18:00
- St: 7:30 – 13:00
- Čt: 7:30 – 15:00
- Pá: 7:30 – 13:00
- Víkendy: dle domluvy

## Technologie
- Čistý HTML/CSS/JS (single file index.html)
- Google Fonts: Syne + Nunito
- Intersection Observer pro fade-up animace
- Google Maps iframe embed

## Repozitář
- GitHub: https://github.com/supercigan/dhobalova
- Vercel: auto-deploy z master branch

## Datum
2026-04-01
