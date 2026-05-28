# Projekt: [PROJEKT_NR] [PROJEKT_NAME]

## Projektdaten
> Bitte vor dem ersten `/lph2` oder `/lph3` ausfüllen

| Feld | Wert |
|---|---|
| Projektnummer | [z.B. (Projekt-Nr.)-25] |
| Projektname | [z.B. Neubau Grundschule {ORTSNAME}] |
| Auftraggeber | [z.B. Stadt {ORTSNAME}] |
| Ort | [z.B. {ORTSNAME}] |
| LPH aktuell | [z.B. LPH 2] |

---

## Claude DOKU System

| Was | Wo |
|---|---|
| LPH 2 Template | `Claude_DOKU\LPH2_Template.html` |
| LPH 3 Template | `Claude_DOKU\LPH3_Template.html` |
| LPH 2 Report (Output) | `Claude_DOKU\LPH2_Report.html` |
| LPH 3 Report (Output) | `Claude_DOKU\LPH3_Report.html` |
| Beteiligtenliste | `Claude_DOKU\` (als PDF ablegen — gilt als Source of Truth) |

---

## Schnellstart

```
/lph2    →  Vorentwurfsbericht (LPH 2)
/lph3    →  Entwurfsplanung (LPH 3) — benötigt fertige LPH2_Report.html
```

Claude Code liest diese Datei automatisch beim Start.
Alle Templates und der Output-Ordner sind lokal in diesem Projekt — kein Desktop, kein anderer Rechner nötig.
