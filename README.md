# Bewerbungs-Panel

Ein Skill für Claude Code. Sieben Claudes versuchen, deine Bewerbung abzulehnen, und danach bekommst du eine verbesserte Fassung.

**Wie es abläuft**

1. Ein Claude spielt das Bewerbungssystem, das aussortiert, bevor ein Mensch liest (Stichwörter, Lesbarkeit, Lücken).
2. Ein zweiter spielt die Personalchefin: Einladen, vielleicht oder Absage.
3. Fünf weitere lesen jeder für sich, als Fachvorgesetzte, Recruiter, stärkerer Mitbewerber, Geschäftsführer und Branchenexperte. Jeder gibt eine Note von 1 bis 10 und nennt die Zeilen, die er streichen würde.
4. Aus allem entsteht eine Tabelle der Absagegründe, mit Zitat aus deinen Unterlagen.
5. Claude baut einen verbesserten Lebenslauf und auf Wunsch ein verbessertes Anschreiben.
6. Zur Gegenprobe lesen Filter und Personalchefin die neue Fassung noch einmal.

**Regeln:** Es wird nichts erfunden. Fehlt eine Zahl, fragt der Skill danach. Deine Unterlagen bleiben auf deinem Rechner.

## Einrichten

Claude Code, Windows (PowerShell):

```powershell
git clone https://github.com/neubauerwilli/bewerbungs-panel "$env:USERPROFILE\.claude\skills\bewerbungs-panel"
```

Mac/Linux:

```bash
git clone https://github.com/neubauerwilli/bewerbungs-panel ~/.claude/skills/bewerbungs-panel
```

Dann in Claude Code sagen: „Prüf meine Bewerbung" und Lebenslauf und Stellenanzeige nennen.

## Ohne Claude Code

Öffne [prompt-zum-einfuegen.md](prompt-zum-einfuegen.md), kopiere den Prompt in einen neuen Chat und hänge Lebenslauf und Anzeige an. Dort laufen die sieben Leser nacheinander statt als getrennte Unteragenten, die Trennung der Urteile ist also schwächer.

## Von

Willi Neubauer, [@willi_neubauer.ai](https://www.instagram.com/willi_neubauer.ai/). Lizenz: MIT, siehe [LICENSE](LICENSE).
