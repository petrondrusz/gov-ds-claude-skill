# Design systém gov.cz — Claude Skill / Prompt

Obsah souboru `prompt.md` proměňuje Clauda v experta na [Design systém gov.cz](https://designsystem.gov.cz) (v4.2.4). Pokrývá jak **vývojářskou implementaci** (web komponenty, tokeny, CSS), tak **Figma design workflow** (grid, breakpointy, spacing, šablony).

## Jak použít

### Claude desktop aplikace (claude.ai)

1. Otevři nebo vytvoř **Project** v Claude desktop appce
2. Klikni na **Project instructions**
3. Zkopíruj celý obsah souboru `prompt.md` a vlož ho do pole instrukcí
4. Uložit — Claude bude v celém projektu fungovat jako expert na gov.cz design systém

### Claude Code (CLI / VS Code / JetBrains)

Zkopíruj `prompt.md` do:
```
~/.claude/commands/gov-ds.md
```
Potom použij příkaz `/gov-ds` v jakémkoli chatu.

---

## Co prompt obsahuje

### Pravidla a povinnosti
| Sekce | Obsah |
|-------|-------|
| Povinnost použití | Pro koho je DS povinný, výjimky, právní základ (zákon č. 365/2000 Sb., usnesení č. 984/2023) |
| Pravidla modifikace | Co smí/nesmí být změněno, jak customizovat přes tokeny |

### Design principy
| Sekce | Obsah |
|-------|-------|
| Barvy | Kompletní palety s hex hodnotami — primary, secondary, neutral, error, warning, success, focus, visited |
| Sémantické tokeny | `--button-*`, `--text-*`, `--border-*`, `--icon-*`, `--interactive-*` |
| Typografie | Škála 13 velikostí (12–56px), Roboto, responsive hodnoty mobile vs. desktop |
| Ikony | Bootstrap Icons + 100+ komplexních gov ikon, `<gov-icon>` |

### Figma & Layout
| Sekce | Obsah |
|-------|-------|
| Figma workflow | Kit struktura (gov-materials, gov-templates, gov-icons), frame setup, variable modes, naming konvence |
| Breakpointy | Mobile < 480px · Tablet 480–1023px · Desktop ≥ 1024px + col-span breakpointy |
| Grid systém | 12 sloupců, `<gov-grid>`, gap hodnoty v px |
| Layout & Container | Max-width 1200px, 5 variant layoutu, šířky sloupců a sidebaru (~312px) |
| Spacing tokeny | `--templates-margin-*` s px hodnotami (responsive) + `--spacing-*` (fixní) |
| Component heights | XS=24px → XL=56px, line-heights, icon sizes, corner radius |

### Komponenty (všech 35)
| Sekce | Obsah |
|-------|-------|
| Všechny komponenty | Accordion, Autocomplete, Banner, Blockquote, Breadcrumbs, Button, Card, Checkbox, Chip, Datepicker, Dialog, Dropdown, Empty, Error Code, File, Flex, Infobar, Input, Link, Loaders, Message, Pagination, Password, Radio, Search, Select, Stepper, Switch, Tabs, Tag, Theme Switch, Tile, Timepicker, Toast, Tooltip, Wizard |
| Helper organismy | Header & Navigation, Footer, Card Grid, Table, Image & Gallery |

Každá komponenta obsahuje: kdy použít · varianty a atributy · HTML příklad · klíčová pravidla.

### Pravidla tvorby
| Sekce | Obsah |
|-------|-------|
| Formuláře | Anatomie, výběr komponent, validace, chybové hlášky |
| IA & Struktura | Informační architektura, postup návrhu struktury |
| Psaní obsahu | Obrácená pyramida, tón, gender neutralita, SEO |
| Přístupnost | WCAG 2.1 A+AA, zákon č. 99/2019 Sb., 4 principy |
| Responsivita | Mobile first, 320px start, touch targety 1×1cm |
| Loga | Pravidla pro gov a EU loga |
| Šablony | 13 šablon, spacing tokeny, Figma naming konvence |

---

## Klíčová čísla

| Parametr | Hodnota |
|----------|---------|
| Grid | 12 sloupců |
| Container max-width | 1200px |
| Two-column breakpoint | 1024px |
| Default section gap | 48px desktop / 42px mobile |
| Page horizontal padding | 24px desktop / 16px mobile |
| Default component height (M) | 40px |
| Base font size | 16px |
| Font | Roboto (povinný) |

---

## Zdroj

Data jsou extrahována z [designsystem.gov.cz](https://designsystem.gov.cz) (verze 4.2.4, březen 2026) a z Figma kitu [gov-templates](https://www.figma.com/community/file/gov-templates).
Vlastník design systému: **Digitální a informační agentura (DIA)** — design@dia.gov.cz
