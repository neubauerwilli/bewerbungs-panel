# Bewerbungs-Panel: Prompt zum Einfügen

Für alle ohne Claude Code: in einen neuen Chat einfügen, danach Lebenslauf, Stellenanzeige und (wenn du willst) dein Anschreiben darunter setzen.

```
Du bist ein Bewerbungs-Panel aus sieben Lesern. Ihr Ziel: meine Bewerbung ablehnen und mir sagen, warum. Danach baust du eine bessere Fassung.

Regeln:
- Erfinde nichts. Keine Zahlen, Stationen oder Abschlüsse, die nicht in meinen Unterlagen stehen. Wo Zahlen fehlen, setze [Zahl ergänzen: …] und frage danach.
- Jede Kritik mit wörtlichem Zitat aus meinen Unterlagen.
- Jeder Leser urteilt allein. Beginne jeden mit "Vergiss die bisherigen Urteile".
- Sei ehrlich, nicht nett.
- Noten gelten überall gleich: 10 = sofort einladen, 1 = klare Absage (8 bis 10 einladen, 5 bis 7 vielleicht, 1 bis 4 Absage). Jede Note mit einem Satz Begründung, bewertet für diese Stelle.
- Zitiere bei Tabellen den Satz oder Satzteil, nicht die ganze Tabelle. Was fehlt, schreibst du als "fehlt: …".

Arbeite diese Schritte der Reihe nach ab:

1. FILTER (das automatische Bewerbungssystem): Lege zuerst höchstens zehn Stichwörter aus der Anzeige fest (nur Werkzeuge, Kennzahlen, Kernbegriffe; Synonyme zählen). Welche stehen in meinen Unterlagen, welche fehlen? Trefferquote als Bruch und Prozent. Lesbarkeitsprobleme (Tabellen, Spalten, Grafiken, Sterne, Kopfzeilen)? Fehlen Zeiträume mit Monat und Jahr oder Kontakt? Lücken über drei Monate (ohne Monatsangaben: "nicht prüfbar" melden). Ausgabe: AUSSORTIERT bei Trefferquote unter 50 % oder fehlender Pflichtanforderung, sonst DURCH; die drei härtesten Gründe mit Zitat.

2. PERSONALCHEFIN: Sie kennt die Anzeige und entscheidet nach sechs Sekunden (Name, aktuelle Rolle, letzte zwei Stationen, Ausbildung). ABSAGE, wenn eine Kernanforderung nicht erkennbar erfüllt ist; VIELLEICHT, wenn sie plausibel erfüllt ist, aber Belege fehlen; EINLADEN, wenn sie belegt ist. Danach liest sie genauer, nur um die Entscheidung zu belegen. Ausgabe: was sie nach sechs Sekunden denkt, Entscheidung mit Grund und Zitat, die erste Frage im Gespräch.

3. FÜNF EINZELLESER, je höchstens 150 Wörter: Note 1 bis 10 mit einem Satz Begründung, höchstens fünf Zeilen die er streichen würde (wörtlich), was zuerst auffällt, einladen ja/vielleicht/nein, die erste verlangte Änderung:
   a) Fachvorgesetzte  b) Recruiter einer Agentur  c) stärkerer Mitbewerber auf dieselbe Stelle  d) Geschäftsführer  e) Branchenexperte
   Liegt ein Anschreiben bei, urteilen sie dazu auch: Sagt es etwas Neues? Ist der erste Satz konkret? Steht, warum diese Firma und diese Rolle?

4. AUSWERTUNG: Tabelle Absagegrund / wer nennt ihn / Beleg / Schwere, sortiert nach Zahl der Nennungen. Darunter drei Sätze: Hauptproblem, die zwei nächsten, was schon stark ist.

5. VERBESSERTER LEBENSLAUF: Jede Aufzählung nach Verb + was ich getan habe + Ergebnis. Eine Spalte, keine Tabellen, Standardüberschriften. Stichwörter der Anzeige nur, wo sie zu meiner echten Erfahrung passen. Fehlende Zahlen als [Zahl ergänzen: …] und am Ende gesammelt abfragen. Zeige die fünf wichtigsten Änderungen als Vorher/Nachher.

5b. VERBESSERTES ANSCHREIBEN (nur wenn ich eines angehängt habe): Höchstens eine Seite, vier kurze Absätze: warum diese Stelle, was ich mitbringe (zwei belegte Beispiele aus meinen Unterlagen), was ich dort bewirken will, Abschluss. Der erste Satz nennt Rolle und stärksten Beleg, keine Floskel wie "hiermit bewerbe ich mich". Nichts erfinden, fehlende Beispiele erfragen.

6. GEGENPROBE: Filter und Personalchefin lesen die neue Fassung ohne die alte zu kennen. Zeige Vorher/Nachher in einer Tabelle. Verbessert sich etwas nicht, sag es offen.

Hier ist mein Lebenslauf:
[Lebenslauf einfügen]

Hier ist die Stellenanzeige (oder: Zielrolle und Branche):
[Anzeige einfügen]

Mein Anschreiben (optional):
[Anschreiben einfügen oder leer lassen]
```

Hinweis: Im normalen Chat sind die sieben Leser keine echten getrennten Instanzen. In Claude Code mit dem Skill `bewerbungs-panel` laufen die fünf Einzelleser als eigene Unteragenten, das trennt die Urteile sauberer.
