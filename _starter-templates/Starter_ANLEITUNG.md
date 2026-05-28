# Claude DOKU Starter — Anleitung

## Was ist das?
Ein portables System zur automatischen Erstellung von LPH 2 und LPH 3 Berichten
für beliebige Architekturprojekte. Einmal kopieren, einmal ausfüllen, fertig.

---

## Einmalig: Für jedes neue Projekt

### Schritt 1 — Ordner kopieren
Diesen ganzen Ordner (`_Claude_DOKU_Starter`) in den neuen Projektordner kopieren.

```
25 - (Projekt-Nr.) Neubau GS {ORTSNAME}\
└── _Claude_DOKU_Starter\        ← hier reinkopieren
    ├── CLAUDE.md
    ├── ANLEITUNG.md
    └── Claude_DOKU\
        ├── LPH2_Template.html
        └── LPH3_Template.html
```

### Schritt 2 — CLAUDE.md ausfüllen
`CLAUDE.md` öffnen und die 5 Felder eintragen:
- Projektnummer
- Projektname
- Auftraggeber
- Ort
- Aktuelle LPH

### Schritt 3 — Beteiligtenliste ablegen
Offizielle Beteiligtenliste als PDF in `Claude_DOKU\` kopieren.
Claude verwendet diese als **Source of Truth** — nur dort aufgeführte Firmen werden in den Report übernommen.

### Schritt 4 — Claude Code öffnen
Claude Code im **Projektordner** öffnen (nicht im Unterordner).
Claude liest `CLAUDE.md` automatisch.

### Schritt 5 — Report starten
```
/lph2    →  LPH 2 Vorentwurfsbericht
/lph3    →  LPH 3 Entwurfsplanung
```
Claude durchsucht selbständig alle Projektdateien (PDF, DOCX, XLSX, Bilder).
Der fertige Report landet in `Claude_DOKU\LPH2_Report.html` bzw. `LPH3_Report.html`.

---

## Enthaltene Dateien

| Datei | Beschreibung |
|---|---|
| `CLAUDE.md` | Projektconfig — Claude liest dies automatisch |
| `ANLEITUNG.md` | Diese Anleitung |
| `Claude_DOKU\LPH2_Template.html` | Leeres HTML-Template für LPH 2 |
| `Claude_DOKU\LPH3_Template.html` | Leeres HTML-Template für LPH 3 |

---

## Report als PDF speichern

1. HTML-Report im Browser öffnen
2. Klicke "Als PDF speichern" (Toolbar oben)
3. Druckdialog: Format **A4 Querformat**, "Hintergrundgrafiken" aktivieren
4. Speichern

---

## Hinweise

- **Kein Desktop nötig** — alles läuft lokal aus dem Projektordner
- **Kein Username** — funktioniert auf jedem Rechner
- **LPH 3 benötigt LPH 2** — erst `/lph2` ausführen, dann `/lph3`
- **Beteiligte**: Nur was in der PDF-Beteiligtenliste steht kommt in den Report
