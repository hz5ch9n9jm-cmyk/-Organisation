# Organisation

Persönliche Werkzeuge als einzelne Web-Seiten. Jede Datei ist die Quelle eines claude.ai-Artifacts
(ohne eigenes `<html>`-Gerüst; das ergänzt die Veröffentlichung).

| Datei | Werkzeug | Live |
|---|---|---|
| `index.html` | Lagezentrum: Tageslage, Aufgaben, Routinen, Woche, Ziele | https://claude.ai/artifact/5BgP95hfCsr8Ebt72iUUjd |
| `objektakte.html` | Objektakte: Immobilien bewerten, Kauf und Vermietung prüfen | https://claude.ai/artifact/Kjhv1zj52LJtkxCb22jqKC |

# Lagezentrum

## Bereiche

| Tab | Inhalt |
|---|---|
| Lage | Ort des Tages (Mo–Fr Standort, Sa–So Zuhause), nächster Schritt unter 5 Minuten, Top 3, Routinen heute, Tagesplan, Losung |
| Aufgaben | Schnellerfassung in den Eingang, Priorität Rot/Gelb/Blau, Ort, Bereich, Fälligkeit, nächster Schritt |
| Routinen | Gewohnheiten mit Wochenraster und Serie, wahlweise täglich, Mo–Fr oder Sa–So |
| Woche | Feste Wochenvorlage, Ort pro Tag umschaltbar, Sonntags-Lage, Packliste |
| Ziele | Ziele mit Etappen, Fortschritt und Frist; Etappe mit einem Tipp als Aufgabe übernehmen |

Dazu: Fokus-Timer (10/25/45 Min), Sicherung als JSON speichern und laden.

## Farbcode

Grün = erledigt · Gelb = Achtung/wichtig · Rot = dringend/überfällig · Blau = Information/normal.

## Speicherung

Als claude.ai-Artifact liegen die Daten privat im eigenen Konto und werden geräteübergreifend abgeglichen.
Ohne Anmeldung fällt die Seite auf den Browser-Speicher zurück.

`index.html` ist die Artifact-Quelle (ohne eigenes `<html>`-Gerüst; das ergänzt die Veröffentlichung).

# Objektakte

Bewertet Immobilien für Kauf und Vermietung und gibt ein Ampel-Urteil: **Kaufen**, **Verhandeln** oder **Finger weg**.

| Bereich | Inhalt |
|---|---|
| Urteil | Vier Prüfpunkte (Preis, Liquidität, Rendite, Risiko), Höchstpreis, Kennzahlen, Monatsrechnung, Warnungen, Stresstest |
| Daten | Objekt, Kaufpreis und Boden, Kaufnebenkosten je Bundesland, Miete und laufende Kosten |
| Finanzen | Eigenkapital, Hauptdarlehen, KfW/zweites Darlehen, Restschuld, Stresstest, Tilgungsplan (CSV) |
| Prognose | Vermögen bei Verkauf über 30 Jahre mit Szenarien gegen ETF-Sparplan, Gewinnzerlegung |
| Check | Makro- und Mikrolage, Besichtigung mit Sanierungskosten, Unterlagen (Wohnung oder Haus) |

Rechenkern (`Rechner` im ersten `<script>`-Block) ohne Abhängigkeiten:

- Grunderwerbsteuer je Bundesland, Stand Oktober 2026
- Instandhaltung nach § 28 II. BV (Werte ab 1.1.2026), Mietausfallwagnis 2 % nach § 29 II. BV
- AfA 2 % / 2,5 % (vor 1925) / 3 % (ab 2023), Inventar über 10 Jahre, 15-%-Grenze für anschaffungsnahen Aufwand
- Annuitätendarlehen monatlich; nach der Zinsbindung tilgt die neue Rate bis zum ursprünglich geplanten Ende
- Eigenkapitalrendite als interner Zinsfuß inkl. Verkauf; ETF-Vergleich mit identischen Einzahlungen
- Spekulationsfrist (10 Jahre) im Verkaufserlös berücksichtigt

Faustregeln, keine Steuer- oder Anlageberatung.
