---
name: bewerbungs-panel
description: Use when eine Bewerbung geprüft und verbessert werden soll — "prüf meine Bewerbung", "prüf meinen Lebenslauf", "warum bekomme ich Absagen", "Bewerbungs-Panel", "Lebenslauf-Check", "ist mein Anschreiben gut genug". Schickt Lebenslauf (und auf Wunsch das Anschreiben) durch sieben getrennte Leser (Bewerbungssystem, Personalchefin, fünf Einzelleser), sammelt die Ablehnungsgründe und baut eine verbesserte Fassung. Nicht zum Erfinden von Berufserfahrung.
---

# Bewerbungs-Panel

Sieben Leser versuchen, eine Bewerbung abzulehnen. Danach steht fest, warum Firmen sie aussortieren würden, und eine verbesserte Fassung liegt vor.

## Grundregeln

- **Nichts erfinden.** Keine Stationen, Zahlen, Abschlüsse oder Programme, die die Unterlagen nicht nennen. Fehlt eine Zahl, setze `[Zahl ergänzen: …]` und frage danach.
- **Jedes Urteil mit Beleg.** Wer etwas kritisiert, zitiert die Zeile wörtlich.
- **Die Leser sind unabhängig.** Ein Leser sieht nie das Urteil eines anderen. Sonst schließen sich alle der ersten Meinung an.
- **Ehrlich, nicht nett.** Ziel ist, die Absage zu finden, bevor eine Firma sie schickt.
- Die Unterlagen bleiben bei dir. Nichts wird hochgeladen oder an Dritte geschickt.

## Schritt 0 — Eingaben

Du brauchst:
1. Den Lebenslauf (Text, Datei oder eingefügt).
2. Die Stellenanzeige, auf die er zielt. Gibt es keine, frage nach Zielrolle und Branche in einem Satz und arbeite damit.
3. Optional das Anschreiben. Liegt eines bei oder wird danach gefragt, läuft Schritt 5b mit.

Mehr fragst du nicht. Fehlt der Lebenslauf, bitte darum und warte.

## Schritt 1 — Der Filter (Leser 1)

Er spielt das automatische Bewerbungssystem, das entscheidet, ob ein Mensch die Bewerbung überhaupt sieht.

Prüft:
- Stichwörter der Anzeige: welche stehen in den Unterlagen, welche fehlen (Liste, wörtlich).
- Lesbarkeit für Maschinen: Tabellen, mehrere Spalten, Grafiken, Icons, Text in Kopf- oder Fußzeile, ungewöhnliche Überschriften.
- Pflichtangaben: Kontakt, Zeiträume, Abschlüsse, Stationen mit Monat und Jahr.
- Lücken über drei Monate ohne Erklärung.

Ausgabe: `DURCH` oder `AUSSORTIERT`, Trefferquote in Prozent, die drei härtesten Gründe, je mit zitierter Stelle.

## Schritt 2 — Die Personalchefin (Leser 2)

Sie entscheidet, ob es ein Gespräch gibt. Sie liest zuerst sechs Sekunden: Name, aktuelle Rolle, die letzten zwei Stationen, Ausbildung. Danach liest sie genauer, falls das Bild trägt.

Ausgabe:
- Was sie nach sechs Sekunden über die Person denkt (ein Satz).
- Entscheidung: `EINLADEN`, `VIELLEICHT` oder `ABSAGE`.
- Der Grund in einem Satz, der Beleg als Zitat.
- Die eine Frage, die sie im Gespräch zuerst stellen würde.

## Schritt 3 — Fünf Einzelleser (Leser 3 bis 7)

Jeder liest allein, nur die Unterlagen und die Anzeige. Keiner sieht Schritt 1 und 2 oder einen anderen Leser.

| Nr. | Rolle | Worauf er achtet |
|---|---|---|
| 3 | Fachvorgesetzte | Kann die Person die Aufgabe? Fehlt Fachliches? |
| 4 | Recruiter einer Agentur | Passt die Geschichte zur Rolle? Wo springt das Interesse ab? |
| 5 | Mitbewerber | Eine stärkere Person auf dieselbe Stelle. Was hat sie, was diese Bewerbung nicht zeigt? |
| 6 | Geschäftsführer | Ergebnisse und Wirkung statt Aufgabenlisten. Lohnt sich die Einstellung? |
| 7 | Branchenexperte | Stimmen Begriffe, Werkzeuge und Niveau der Branche? |

Jeder liefert:
- Note 1 bis 10.
- Die Zeilen, die er streichen würde, wörtlich zitiert.
- Was zuerst auffällt (gut oder schlecht).
- Würde er einladen: ja, vielleicht, nein.
- Die erste Änderung, die er verlangen würde.

**In Claude Code:** starte die fünf als getrennte Unteragenten parallel (`Agent`, Modell `sonnet`), jeden mit nur den Unterlagen, der Anzeige und seiner Rolle.
**Im normalen Chat:** arbeite die fünf nacheinander ab. Beginne jeden mit „Vergiss die bisherigen Urteile, du bist neu in der Rolle". Sage dem Nutzer, dass die Trennung hier schwächer ist als mit echten Unteragenten.

## Schritt 4 — Auswertung

Fasse die sieben Urteile zu einer Tabelle zusammen:

| Absagegrund | Wer nennt ihn | Beleg aus den Unterlagen | Schwere |
|---|---|---|---|

Gruppiere gleiche Punkte. Sortiere nach Zahl der Leser, die ihn nennen. Darunter in drei Sätzen: das Hauptproblem, die zwei nächsten, und was schon stark ist (nenne es, damit es bei der Überarbeitung bleibt).

## Schritt 5 — Verbesserter Lebenslauf

Baue den Lebenslauf neu, jede Aufzählung nach dem Muster **Verb + was du getan hast + Ergebnis**. Beispiel: „Aufbau eines Kundenportals, Bearbeitungszeit von 5 auf 2 Tage gesenkt."

Regeln:
- Eine Spalte, keine Tabellen, keine Grafiken, Standardüberschriften (Berufserfahrung, Ausbildung, Kenntnisse).
- Stichwörter der Anzeige nur dort einbauen, wo sie zur echten Erfahrung passen.
- Stärkste Stationen und Ergebnisse nach oben, Schwaches kürzen.
- Wo Zahlen fehlen: `[Zahl ergänzen: …]`. Liste diese Stellen am Ende gesammelt auf und frage, ob der Nutzer sie nennt.
- Nichts hinzufügen, was nicht belegt ist.

Speichere als `lebenslauf-verbessert.md` im Arbeitsordner und zeige die fünf wichtigsten Änderungen als Vorher/Nachher.

## Schritt 5b — Anschreiben (nur wenn eines vorliegt oder gewünscht ist)

Die fünf Einzelleser lesen das Anschreiben mit und urteilen zusätzlich: Sagt es etwas, das nicht schon im Lebenslauf steht? Ist der erste Satz konkret? Steht, warum diese Firma und diese Rolle?

Schreibe es neu:
- Maximal eine Seite, vier kurze Absätze: warum diese Stelle, was du mitbringst (zwei belegte Beispiele aus den Unterlagen), was du dort bewirken willst, Abschluss.
- Erster Satz nennt Rolle und den stärksten Beleg, keine Floskel wie „hiermit bewerbe ich mich".
- Nichts erfinden. Fehlen Beispiele, frage danach.

Speichere als `anschreiben-verbessert.md`. Liegt kein Anschreiben vor und es wird nicht gewünscht, überspringe den Schritt.

## Schritt 6 — Gegenprobe

Lasse Leser 1 und Leser 2 die neue Fassung noch einmal lesen, ohne die alte zu kennen. Zeige:

| | Vorher | Nachher |
|---|---|---|
| Filter | Trefferquote, Ergebnis | … |
| Personalchefin | Entscheidung | … |

Verbessert sich ein Wert nicht, sage das offen und nenne den Grund. Dann bekommt der Nutzer die Liste der offenen Punkte zurück, statt einer geschönten Zusammenfassung.

## Abschluss

Nenne in drei Zeilen: wichtigste Ablehnungsgründe, was geändert wurde, was der Nutzer selbst beisteuern muss (die `[Zahl ergänzen]`-Stellen). Biete an, dasselbe Panel für ein LinkedIn-Profil laufen zu lassen.
