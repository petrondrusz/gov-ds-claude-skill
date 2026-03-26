# Design systém gov.cz — Claude Skill / Prompt

Obsah souboru `prompt.md` proměňuje Clauda v experta na [Design systém gov.cz](https://designsystem.gov.cz) (v4.2.4).

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

| Sekce | Obsah |
|-------|-------|
| Povinnost použití | Pro koho je DS povinný, výjimky, právní základ |
| Pravidla modifikace | Co smí/nesmí být změněno, jak customizovat |
| Barvy | Kompletní palety s hex hodnotami (primary, secondary, neutral, error, warning, success, focus, visited) |
| Sémantické tokeny | `--button-*`, `--text-*`, `--border-*`, `--icon-*` |
| Typografie | Škála 13 velikostí, Roboto, CSS třídy a proměnné |
| Velikostní tokeny | Spacing, component height, icon size, template margins |
| Ikony | Bootstrap Icons + komplexní gov ikony, `<gov-icon>` |
| Komponenty | Accordion, Button, Card, Input, Dialog — s HTML příklady |
| Formuláře | Anatomie, výběr komponent, validace, chybové hlášky |
| IA & Struktura | Informační architektura, postup návrhu struktury |
| Psaní obsahu | Obrácená pyramida, tón, gender neutralita, SEO |
| Přístupnost | WCAG 2.1 A+AA, zákon č. 99/2019 Sb. |
| Responsivita | Mobile first, 320px breakpoint, touch targety |
| Loga | Pravidla pro gov a EU loga |
| Šablony | Struktury, spacing tokeny, Figma naming konvence |

---

## Zdroj

Data jsou extrahována z [designsystem.gov.cz](https://designsystem.gov.cz) (verze 4.2.4, březen 2026).
Vlastník design systému: **Digitální a informační agentura (DIA)** — design@dia.gov.cz
