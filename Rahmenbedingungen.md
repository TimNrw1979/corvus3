# Band 2 – Rahmenbedingungen

> Referenzdokument: Festgelegte Prinzipien, Konventionen und Entscheidungen,
> die für das neue Projekt verbindlich übernommen werden.

---

## Stilprinzipien

1. **Kein emotionales Überkommentieren** – Emotionen, die bereits durch Haltung,
   Handlung oder Dialog sichtbar sind, werden nicht benannt. Was gezeigt wird,
   wird nicht erklärt.

2. **Wiederholungen vermeiden** – Insbesondere „er wusste", „er verstand",
   „er wartete". Konstruktionen wie doppelte Verbmuster oder gedankenparallele
   Wiederholungen werden aufgelöst. Anker-Sätze (bewusste Wiederholungen als
   Stilmittel) werden sparsam gesetzt und brauchen Abstand voneinander.

3. **Satzrhythmus in Höhenmomenten** – Kurze Sätze, wenig Nebensätze, kein
   erklärender Nachsatz. Ein starkes Bild steht für sich.

4. **Figureneinsichten durch Wahrnehmung, nicht Reflexion** – Wenn eine Figur
   eine Erkenntnis über eine andere hat, zeigt sich das in einer konkreten
   Erinnerung, Beobachtung oder Handlung — nicht in einem zusammenfassenden
   Schluss. Der Leser zieht die Schlussfolgerung selbst.

5. **Figuren erklären nicht, was sie denken** – Besonders bei Antagonisten-POVs
   (Marre): Beobachtungen und Schlüsse werden nebeneinander gestellt, nicht
   ausformuliert verbunden. Die Lücke zwischen Beobachtung und Konsequenz ist
   beabsichtigt und trägt Spannung.

6. **Schlussformulierungen tragen sich allein** – Ein starker Abschluss (Satz,
   Szene, Kapitel) braucht keine vorbereitende Zusammenfassung. Was der Leser
   aus dem Vorherigen gezogen hat, muss nicht wiederholt werden.

---

## Sprach- und Benennungskonventionen

- **„Dämon"** = Matthews innere Natur (Selbstwahrnehmung, Patricks Blick)
- **„Modus"** = der aktivierte Zustand, von außen beobachtet (Liam, Edmund, Erzähler in Aktionsszenen) — nie beides verwechseln
- **Anrede:** Nur Patrick nennt Matthew „Matthew". Alle anderen: „Mat." Ausnahmen nur mit starker dramaturgischer Begründung.

---

## Datei- und Formatkonventionen (Obsidian/Markdown)

**YAML-Frontmatter:**
```yaml
---
tags:
  - personen
status: in-arbeit
verknüpft:
  - "[[Matthew Ashford]]"
---
```
- Delimitoren: `---` (nie `-----`)
- `tags` und `verknüpft` als eingerückte Listen
- Alle anderen Felder als flache Key-Value-Paare

**Szenendateien:**
- Kein `title`-Feld im YAML-Frontmatter
- Nur `###` als Abschnittstrenner innerhalb einer Szene
- `---` ausschließlich zur Trennung des Einleitungsblocks (Szenentitel + Einordnung) vom Fließtext

**Charakter-Profile (aus Band 1 übernommen):**
- Kursive Quellennotiz unter Abschnittsüberschriften für geerbte Inhalte
- Eigener Abschnitt mit klarer Überschrift für Band-2-Ergänzungen

---

## Serienkonventionen

- **Serienname:** Corvus — typografisch durch Zeilenbruch-Hierarchie vom Bandtitel getrennt, kein Trennzeichen
- **Caldermoor-Vorfall:** Reserviert für einen späteren Band, wird in Band 2 nicht aktiv angegangen
- **Marres Niederlage:** Reserviert für Band 3 — er wird in Band 2 sichtbar, aber nicht besiegt

---

## Editorische Arbeitsweise

- Iterativ: Änderungen in Obsidian → Datei hochladen → Verifikation
- Jeweils ein Element abschließen, bevor das nächste beginnt
- Minimale, chirurgische Eingriffe bevorzugt — Auslassung vor Ersatz bei Erklärungssprache
- Claude übernimmt bei offenen Einzelheiten konkrete Vorschläge statt offener Optionslisten
- Claude nimmt eine konstruktiv-kritische Redaktionsrolle ein: dramaturgische Schwächen benennen, Stilprinzipverstöße markieren, strukturelle Risiken ansprechen — auch wenn Tim bereits in eine Richtung investiert ist
- Bewusste Lücken und ungelöste Elemente sind intentional und werden nicht vorzeitig aufgelöst

---

## Externe Reviewerpraxis

Google Gemini, Copilot, ChatGPT und NotebookLM werden als externe Lektoren eingesetzt. Befunde werden kritisch triagiert: valide Beobachtungen von Halluzinationen oder Fehllesungen intentionaler Entscheidungen trennen.
