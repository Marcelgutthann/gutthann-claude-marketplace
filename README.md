# Gutthann Claude Marketplace

> Claude Code Plugins fuer Architektur- und Planungsbueros - HOAI-konform, druckfest, dokumentationssicher.

Entwickelt von **Gutthann HIW Architekten GmbH** aus echter Projektpraxis. Alle Plugins sind generisch und ohne projektspezifische Daten.

---

## Verfuegbare Plugins

Jede LPH ist ein **eigenes Plugin** mit eigener Versionierung. Kunden installieren nur was sie brauchen.

| Plugin | Slash-Command | Version | Zweck |
|---|---|---|---|
| **lph-1** | `/lph1` | v1.0.0 | LPH 1 Grundlagenermittlung (HOAI Paragraph 33) |
| **lph-2** | `/lph2` | v1.0.0 | LPH 2 Vorentwurfsplanung |
| **lph-3** | `/lph3` | v1.0.0 | LPH 3 Entwurfsplanung |
| **lph-4** | `/lph4` | v1.0.0 | LPH 4 Genehmigungsplanung |
| **lph-5** | `/lph5` | v1.0.0 | LPH 5 Ausfuehrungsplanung |
| **lph-6** | `/lph6` | v1.0.0 | LPH 6 Vorbereitung der Vergabe |
| **lph-7** | `/lph7` | v1.0.0 | LPH 7 Mitwirkung bei der Vergabe |
| **lph-8** | `/lph8` | v1.0.0 | LPH 8 Objektueberwachung |
| **skillboard** | `/projekt-historie` `/dashboard` `/fachplaner-analyse` | v3.1.0 | Wissensbasis pflegen + monochromes Dashboard + Multi-Persona-Fachplaner-Analyse |
| **projektsteuerung-bau** | (Skill) | v1.0.0 | Projektsteuerung Bauprojekte |
| **vgv** | `/vgv` | v1.0.0 | VGV-Analyse: Vertragsrisiko- und Vergabe-Bewertung bei oeffentlichen Verfahren |
| **nachtrag-skill** | `/nachtrag` (+ Auto-Skill) | v1.0.0 | Rechtssichere Nachtraege zu Architektenvertraegen (HAV-KOM / AVB / ZVB / HOAI) |

---

## Installation (fuer Endnutzer)

In Claude Code im Terminal:

```
/plugin marketplace add github:Marcelgutthann/gutthann-claude-marketplace
```

Dann selektiv installieren (nur was du brauchst):

```
/plugin install lph-2
/plugin install lph-3
/plugin install skillboard
```

Nach der Installation: Claude Code einmal neu starten. Danach stehen die Befehle (`/lph2`, `/dashboard`, etc.) projektweit zur Verfuegung.

### Updates

```
/plugin marketplace update gutthann-claude-marketplace
```

Holt automatisch die neuesten Versionen aller installierten Plugins.

---

## Plugin-Repos (eigenstaendig)

Jedes Plugin lebt in einem eigenen Repository - das ermoeglicht unabhaengige Versionierung:

- [gutthann-lph-1](https://github.com/Marcelgutthann/gutthann-lph-1)
- [gutthann-lph-2](https://github.com/Marcelgutthann/gutthann-lph-2)
- [gutthann-lph-3](https://github.com/Marcelgutthann/gutthann-lph-3)
- [gutthann-lph-4](https://github.com/Marcelgutthann/gutthann-lph-4)
- [gutthann-lph-5](https://github.com/Marcelgutthann/gutthann-lph-5)
- [gutthann-lph-6](https://github.com/Marcelgutthann/gutthann-lph-6)
- [gutthann-lph-7](https://github.com/Marcelgutthann/gutthann-lph-7)
- [gutthann-lph-8](https://github.com/Marcelgutthann/gutthann-lph-8)
- [gutthann-skillboard](https://github.com/Marcelgutthann/gutthann-skillboard)
- [gutthann-projektsteuerung](https://github.com/Marcelgutthann/gutthann-projektsteuerung)
- [gutthann-vgv](https://github.com/Marcelgutthann/gutthann-vgv)
- [gutthann-nachtrag](https://github.com/Marcelgutthann/gutthann-nachtrag)

---

## Starter-Templates

Im Unterordner `_starter-templates/` findest du:
- `CLAUDE_Projekt_Template.md` - Vorlage fuer projekt-spezifische CLAUDE.md
- `Starter_ANLEITUNG.md` - Anleitung wie ein neues Projekt aufgesetzt wird

---

## Output-Konvention (verbindlich fuer ALLE Plugins)

Alle Plugins schreiben **ausschliesslich** in einen einzigen Ordner namens `Claude/` im Projekt-Root. Die bestehende Projekt-Struktur wird **nicht angefasst**.

```
<dein-Projekt-Ordner>/                    <- bleibt komplett unveraendert
├── (deine bestehende Struktur)
│
└── Claude/                               <- EINZIGER neuer Ordner
    ├── Projekt_Historie.md
    ├── LPH_1/ ... LPH_8/
    ├── Dashboard/
    └── Fachplaner-Analyse/
```

Du kannst den `Claude/`-Ordner jederzeit komplett loeschen - dann ist alles Plugin-generierte weg, deine Projektdateien sind unberuehrt.

## Nutzungs-Voraussetzungen

- Claude Code installiert (https://claude.com/claude-code)
- Anthropic API-Account (eigener Account, eigene API-Kosten)
- Pro Projekt eine `CLAUDE.md` mit Projektdaten
- Pflicht-Dateien im Projekt (siehe jeweilige Plugin-Dokumentation)

---
