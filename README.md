# Orbeo: landing di prova con taste-skill

Landing page di prova per un SaaS fittizio (**Orbeo**, monitoraggio siti per web agency), costruita seguendo
[taste-skill](https://github.com/Leonxlnx/taste-skill) v2.5.1 (commit f6b7657). Brief e fatti in `BRIEF.md`.

## Aprirla in locale

Serve un piccolo server (i moduli JS non partono da `file://`):

```bash
python3 -m http.server 8000
# poi apri http://localhost:8000
```

## Struttura

- `index.html`: la pagina (testi in italiano, palette teal-on-paper, font Outfit).
- `assets/`: il kit di taste-skill copiato per intero, così la pagina si può modificare e ricontrollare con gli script della skill. La pagina ne usa circa 40 file.
- `.taste-skill/`: storico dei deal, waiver e stato del gate.
- `screenshots/`: la pagina intera a 1440 px e a 390 px.
- `names.json`: la ricerca fatta sul nome coniato.

## Esito dei controlli della skill

`GATE: OPEN 1` (tre giri usati): resta un vuoto nella sezione prezzi su telefono.
Waiver (in `.taste-skill/waivers.json`): titoli italiani non riconosciuti dal controllo `copy-headings`, FAQ senza immagini,
due comportamenti dei diagrammi del kit. Layout pulito a 1440, 1024, 820, 768 e 390; `copy-lint` e `perf` senza errori.

## Licenza

Il kit in `assets/` è di taste-skill (licenza in `LICENSE-taste-skill`). Nomi, prezzi e dati di Orbeo sono inventati per la prova.
