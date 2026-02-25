# Begriffsdefinitionen / Glossar (Workshop-Demo)
## CustomGPT „Prüfung von Arzneimittelbezeichnungen“ – Demo-Material

> Hinweis: Dieses Glossar ist ein **fiktives Workshop-Beispiel** und dient nur zur Demonstration von strukturiertem Prompting und nachvollziehbarer Begriffsverwendung.

---

## Zweck des Glossars
Dieses Glossar unterstützt die einheitliche Verwendung von Begriffen in:
- Vorprüfungen von Arzneimittelbezeichnungen
- Prüfberichten
- Entwürfen von Abschlussschreiben
- internen fachlichen Rückfragen

---

## Begriffe (alphabetisch)

### Abschlussschreiben (Entwurf)
Ein formaler Textentwurf zur Mitteilung eines Prüfergebnisses oder Zwischenstands.  
Im Kontext dieses Demo-Systems ist ein Abschlussschreiben **immer als Entwurf** zu verstehen und ersetzt keine finale Freigabe.

**Wichtig:**  
- neutraler Stil  
- nachvollziehbare Begründung  
- keine rechtsverbindliche Entscheidung simulieren

---

### Antrag-ID
Eindeutige Kennung eines Vorgangs / Antrags im Fachprozess.

**Beispiel:** `A-2026-0142`

**Verwendung im Prüfbericht:**  
Zur eindeutigen Zuordnung des Falls.

---

### Antragsteller
Organisation oder Unternehmen, das den Antrag eingereicht hat.

**Beispiel:** `Beispiel Pharma GmbH`

---

### Befund
Strukturierte Feststellung im Rahmen der Vorprüfung (z. B. „Angabe vorhanden“, „unklar“, „Regelbezug nicht belegbar“).

**Abgrenzung:**  
Ein Befund ist **keine finale Entscheidung**.

---

### Begründung (fachlich)
Nachvollziehbare Erläuterung, warum ein Befund oder eine Einschätzung getroffen wurde.

**Qualitätsanforderung (Demo):**
- bezieht sich auf konkrete Falldaten
- verweist auf bereitgestellte Regeln / Kriterien (wenn vorhanden)
- markiert Unsicherheiten

---

### Datenlage
Einschätzung, wie vollständig und belastbar die bereitgestellten Falldaten für eine Vorprüfung sind.

**Beispielkategorien (Demo):**
- vollständig
- teilweise vollständig
- unzureichend

---

### Evidenz aus Falldaten
Die konkret im Fall vorhandenen Informationen, auf die sich ein Befund stützt.

**Beispiel:**  
`produktname vorhanden`, `sprachversion = de`, `wirkstoff nicht angegeben`

---

### Falldaten
Die vom Nutzer bereitgestellten strukturierten Informationen zu einem konkreten Prüfobjekt.

**Typische Felder (Demo):**
- antrag_id
- produktname
- wirkstoff
- verfahrensart
- antragsteller
- sprachversion
- eingangsdatum
- status
- bearbeiter
- weitere_hinweise

---

### Feldmapping
Dokumentierte Zuordnung von Feldern aus einem Export (z. B. CSV) zu den vom Prompt oder Prüfbericht verwendeten Bezeichnungen.

**Ziel:**  
Konsistente Verarbeitung und Nachvollziehbarkeit bei wechselnden Exportformaten.

---

### Guideline-Regelbezug
Verweis auf eine bereitgestellte Regel / ein Kriterium, das für die Vorprüfung verwendet wurde.

**Wichtig:**  
Wenn kein passender Regelbezug im bereitgestellten Material vorhanden ist, muss dies als  
**„nicht belegt“** oder **„kein passender Regelbezug auffindbar“** markiert werden.

---

### Human Review / manuelle Fachprüfung
Verpflichtende fachliche Prüfung durch qualifiziertes Personal vor finaler Bewertung oder Freigabe.

**Grundsatz im Demo-System:**  
Die KI unterstützt nur die **Vorprüfung** und Entwurfsformulierung.

---

### Irreführung (Bezeichnungsprüfung, Demo-Begriff)
Hinweis darauf, dass eine Bezeichnung potenziell missverständlich oder inhaltlich fehlleitend wirken könnte.

**Hinweis:**  
Im Demo-System erfolgt keine abschließende rechtliche Bewertung, sondern nur eine strukturierte Vorprüfung auf Basis bereitgestellter Informationen.

---

### Kurzfazit (Vorprüfung)
Zusammenfassender Abschnitt im Prüfbericht mit:
- vorläufiger Einordnung
- zentralen Begründungspunkten
- Einschränkungen / Unsicherheiten

**Wichtig:**  
Das Kurzfazit ist keine finale Entscheidung.

---

### Offene Punkte
Aspekte, die für eine belastbare Bewertung fehlen oder manuell geprüft werden müssen.

**Beispiele:**
- fehlende Pflichtfelder
- unklarer Regelbezug
- fehlende Vergleichsdaten
- mehrdeutige Formulierung

---

### Produktname (beantragte Bezeichnung)
Die im Fall zu prüfende Arzneimittelbezeichnung.

**Beispiel:** `Cardiolenta`

---

### Prüfkriterium
Ein fachlicher Prüfpunkt, der aus einem Prüfschema oder einer Guideline abgeleitet wird.

**Beispiele (Demo):**
- Irreführung vermeiden
- Verwechslungsgefahr prüfen
- Begründung nachvollziehbar dokumentieren

---

### Prüfbericht (Vorprüfung)
Strukturierte Ausgabe der KI-Unterstützung zur Vorprüfung eines Falls.

**Standardbestandteile (Demo):**
1. Fallüberblick  
2. Vollständigkeitsprüfung  
3. Prüfkriterien mit Befund  
4. Kurzfazit (Vorprüfung)  
5. Offene Punkte für manuelle Fachprüfung  
6. Hinweis zur finalen Prüfung

---

### Sprachversion
Sprachkontext des Falls / der Bezeichnung / des Verfahrens (z. B. `de`, `en`).

**Hinweis:**  
Kann relevant sein für Schreibweise, Verständlichkeit und formale Textentwürfe.

---

### Unsicherheit / Hinweis
Kennzeichnung eines Aspekts, der aufgrund unvollständiger Daten oder fehlender Regeln nicht belastbar bewertet werden kann.

**Beispiel-Formulierungen:**
- „nicht belegt“
- „nicht angegeben“
- „manuelle Klärung erforderlich“

---

### Verfahrensart
Art des Verfahrens (z. B. national, europäisch, Variation etc. – im Workshop als Freitext oder definierte Liste nutzbar).

**Beispiel (Demo):** `national`

---

### Verwechslungsgefahr (Demo-Begriff)
Hinweis auf mögliche Ähnlichkeit oder Verwechselbarkeit mit anderen Bezeichnungen.

**Wichtig:**  
Eine belastbare Bewertung kann zusätzliche Referenzdaten erfordern (z. B. Datenbankabgleich), die im Demo-System ggf. nicht vorliegen.

---

### Vollständigkeitsprüfung
Erster Schritt der Vorprüfung: Prüfung, ob erforderliche Falldaten vorhanden, leer oder unklar sind.

**Ziel:**  
Einschätzen, ob eine Vorprüfung sinnvoll möglich ist und welche Nachforderungen nötig sind.

---

### Wirkstoff
Im Fall angegebener Wirkstoffbezug des Produkts.

**Hinweis:**  
Fehlende Wirkstoffangaben können die Aussagekraft der Vorprüfung einschränken.

---

## Formulierungshilfen für das System (empfohlen)
Diese Formulierungen dürfen bevorzugt verwendet werden:

- „Im Rahmen der Vorprüfung …“
- „Auf Basis der bereitgestellten Informationen …“
- „Ein abschließender Befund ist derzeit nicht möglich, da …“
- „Manuelle Fachprüfung erforderlich für …“
- „Kein passender Regelbezug im bereitgestellten Material auffindbar.“

---

## Nicht empfohlene Formulierungen (für Demo-System)
- „abschließend entschieden“
- „eindeutig zulässig“ (ohne Beleg)
- „rechtsverbindlich festgestellt“
- „final genehmigt / final abgelehnt“

---

## Versionshinweis (Workshop)
- Version: 1.0 (Demo)
- Stand: Workshop-Material (fiktiv)