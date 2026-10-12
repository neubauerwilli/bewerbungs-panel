# Bewerbungs-Panel

Sieben Claude-Perspektiven suchen Schwachstellen in deiner Bewerbung. Danach bekommst du einen überarbeiteten Lebenslauf und auf Wunsch ein Anschreiben.

**[Skill herunterladen](https://willineubauer.com/downloads/bewerbungs-panel.zip)** · **[Kurzanleitung](https://willineubauer.com/bewerbung/)**

## In Claude verwenden
ZIP herunterladen. In Claude unter **Customize > Skills > + > Create skill > Upload a skill** hochladen und aktivieren. Code execution muss aktiviert sein. Danach Lebenslauf und Stellenanzeige anhängen und „Nutze den Bewerbungs-Panel-Skill“ schreiben. [Offizielle Anleitung](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

## In Claude Code verwenden
Ordner `bewerbungs-panel` aus der ZIP entpacken und unter `~/.claude/skills/` ablegen. `SKILL.md` liegt direkt in `~/.claude/skills/bewerbungs-panel/`. Alternativ mit installiertem Git:

Windows (PowerShell):
```powershell
git clone https://github.com/neubauerwilli/bewerbungs-panel "$env:USERPROFILE\.claude\skills\bewerbungs-panel"
```
Mac/Linux:
```bash
git clone https://github.com/neubauerwilli/bewerbungs-panel ~/.claude/skills/bewerbungs-panel
```
Vorhandene Installation nicht erneut klonen oder ungeprüft überschreiben. Dann in Claude Code `/bewerbungs-panel` aufrufen und die Dateien nennen. [Offizielle Skill-Dokumentation](https://code.claude.com/docs/en/skills).

## Ergebnis
Filter → Personalchefin → fünf Perspektiven → Kritik mit Belegen → Überarbeitung → Gegenprobe. In Claude Code arbeiten die fünf Einzelleser als getrennte Unteragenten, sofern verfügbar. Im normalen Chat sind es nacheinander simulierte Rollen. Der Skill ist kostenlos; Claude-Zugang und Nutzungslimits gelten separat.

## Was das Versprechen bedeutet
Der Skill zeigt mögliche Schwachstellen. Er kennt keine tatsächlichen früheren Absagegründe, testet kein echtes ATS und garantiert keine Einladung. Fehlende Erfahrung lässt sich nicht durch bessere Formulierungen ersetzen. Offene Angaben bleiben markiert. Eingelesene Inhalte werden durch den verwendeten KI-Dienst verarbeitet; dies ist kein Offline-Werkzeug. Der Skill versendet keine Bewerbungen.

Ohne Installation: [Prompt zum Einfügen](prompt-zum-einfuegen.md) im neuen Chat verwenden.

## Prüfstand · 12.10.2026
Regeln geprüft und korrigiert; Downloadstruktur und Links technisch geprüft. Ein echter Claude-Modelltest der aktuellen Fassung wurde mangels Anmeldung nicht durchgeführt. Simulierte Perspektiven sind keine Arbeitgebertests.

Von Willi Neubauer · [Kurs-Warteliste: dein eigenes KI-Team](https://willineubauer.com/#warteliste) · Kurs in Arbeit. Lizenz: [MIT](LICENSE).
