# Kapitel-Struktur-Anweisungen — Corvus · Buch 2

> Verbindliche Vorlage für alle ausgearbeiteten Kapitel.  
> Abgeleitet aus: *Kapitel 01 – Morgen*

---

## 1. YAML-Frontmatter

Jedes Kapitel beginnt mit einem YAML-Block. Pflichtfelder:

```yaml
---
tags:
  - buch
  - kapitel
  - akt-i        # akt-i / akt-ii / akt-iii je nach Einordnung
status: ausgearbeitet
verknüpft:
  - "[[Figurenname]]"
  - "[[Weltnotizen]]"
  - "[[Personen]]"
---
```

- Kein `title`-Feld im YAML
- `verknüpft` listet alle im Kapitel aktiven Hauptfiguren sowie `[[Weltnotizen]]` und `[[Personen]]`

---

## 2. Kapitel-Einleitung (nach dem Frontmatter)

Direkt nach dem schließenden `---` folgen drei Elemente in dieser Reihenfolge:

### 2a. Kursive Zusammenfassung (Blockquote)

Eine einzeilige inhaltliche Zusammenfassung als Blockquote. Stil: knapp, beschreibend, ohne Wertung.

```markdown
> Kapitel · [Kurzbeschreibung des Kapitels – Ort, Figuren, Ton, kein Konflikt-Spoiler]
```

Beispiel aus Kapitel 01:
```markdown
> Kapitel · Morgenstille auf Ravenscroft. Drei Perspektiven, ein Tisch, kein Konflikt – nur Ankommen.
```

### 2b. Horizontale Linie

```markdown
---
```

### 2c. Kapitelüberschrift (H1)

Der Kapitelname als einzige H1-Überschrift im Dokument.

```markdown
# Kapitelname
```

---

## 3. Kapitelzitat

Direkt unter der H1, ein einzelner Satz oder kurzer Ausdruck im Pandoc-Custom-Style-Block:

```markdown
::: {custom-style="Kapitelzitat"}
[Zitattext]
:::
```

- Der Satz ist ein wörtliches Zitat aus dem Kapitel selbst — kein frei formulierter, nur sinngemäßer Ersatz.
- Keine Quellenangabe, keine Anführungszeichen
- Er fungiert als emotionaler oder thematischer Verdichter des Kapitels

---

## 4. Gliederung durch Trenner

Kapitel verwenden **keine Abschnittsüberschriften (H2 oder H3)**. Der einzige Titel im Dokument ist die H1-Kapitelüberschrift.

Die innere Gliederung erfolgt ausschließlich über Trenner-Marker:

**Abschnittstrenner** — für stärkere thematische oder zeitliche Einschnitte:

```
!!TRENNUNG_ABSCHNITT!!
```

**Szenentrenner** — für weichere Übergänge innerhalb desselben Handlungsbogens:

```
!!TRENNUNG_SZENE!!
```

Beide Marker stehen als eigene Zeile im Fließtext, ohne Überschrift davor oder danach.

---

## 5. Perspektivstruktur

- **Kein expliziter POV-Header** – der Perspektivwechsel ergibt sich aus der Erzählhaltung und dem fokussierten Bewusstsein
- Die Perspektive folgt immer einer Figur vollständig bis zum nächsten `!!TRENNUNG_SZENE!!` oder `!!TRENNUNG_ABSCHNITT!!`
- Rückblenden oder Zeitsprünge werden innerhalb des Fließtexts angekündigt (nicht per Header), z. B.:
  > *Der Zeitsprung kam ohne Ankündigung – so wie morgens alles kam auf Ravenscroft, bevor der Tag eine Form angenommen hatte.*

---

## 6. Gesamtstruktur auf einen Blick

```
[YAML-Frontmatter]
---
> Kapitel · [Kurzbeschreibung]
---
# Kapitelname
::: {custom-style="Kapitelzitat"}
[Zitattext]
:::

[Fließtext – Szene 1]

!!TRENNUNG_SZENE!!

[Fließtext – Szene 2]

!!TRENNUNG_ABSCHNITT!!

[Fließtext – Szene 3]

!!TRENNUNG_ABSCHNITT!!

[Fließtext – letzte Szene]
```

---

## 7. Was *nicht* verwendet wird

- Keine H2- oder H3-Überschriften innerhalb des Kapitels
- Keine expliziten POV-Header (z. B. `## Matthews Perspektive`)
- Kein `title:`-Feld im YAML
- Keine Nummerierung in Kapitelüberschriften (die Nummerierung steckt im Dateinamen)
- Keine Trennlinien (`---`) innerhalb des Prosatexts (nur im Kopfbereich)

---

## 8. Dateiname-Konvention

```
Kapitel XX - Titel.md
```

Beispiel: `Kapitel 01 - Morgen.md`, `Kapitel 02 - Abend.md`

- Zweistellige Nummerierung mit führender Null
- Titel entspricht der H1-Überschrift im Dokument
