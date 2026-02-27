# Wissenschaftliche Wissensaufbereitung mit GenAI -- Workshop 2 Repository

![Status](https://img.shields.io/badge/status-active-blue)
![Focus](https://img.shields.io/badge/focus-scientific%20evidence-critical)
![License](https://img.shields.io/badge/license-internal-lightgrey)

Repository für evidenzpflichtige, auditierbare KI-Workflows in der wissenschaftlichen Wissensaufbereitung  
(insbesondere regulierte Kontexte wie Pharma, Behörden, Qualitätsdokumentation).

**Schwerpunkt:** Evidence-first Prompting · strukturierte Outputs · Verifier-Logik · Traceability

---

## Quick Start – Wissenschaftliches Arbeiten mit GenAI

**Grundprinzip:**  
> Nur belegen, was im Input steht – alles andere ist UNBEKANNT.

1. Output-Struktur vorab definieren (Schema-first)
2. Jede Kernaussage mit Evidence Snippet + Location versehen
3. Fakten und Interpretation strikt trennen
4. Fehlende Information explizit als `UNBEKANNT` kennzeichnen
5. Verifier-Step verpflichtend bei Zahlen & Compliance-Bezug

---

## Methodischer Kern

### 1. Evidenzpflicht

- Jede relevante Aussage benötigt:
  - Zitat (Evidence Snippet)
  - Fundstelle (Dokument / Seite / Zeile)
- Keine erfundenen Zahlen, Quellen oder Normen
- Keine impliziten Ergänzungen

---

### 2. Delimiter-Architektur

Konsequente Trennung von Input und Arbeitsanweisung:
<<<INPUT>>>
...
<<<END>>>

Verhindert Kontextvermischung und reduziert Halluzinationen.

---

### 3. Schema-first-Prinzip

Erst Output-Format festlegen, z. B.:

- JSON-Struktur
- Bewertungstabelle
- Requirement-Matrix
- Findings Log
- Konfliktprotokoll

Dann Verarbeitung des Inputs.

---

### 4. Verifier-Logik (Guardrail)

Zweiter Prompt als Prüfinstanz:

- Aussage gegen Originaltext abgleichen
- Status: `belegt` / `unbelegt`
- Korrektur + Fundstelle angeben
- „No answer allowed“, wenn keine Evidenz vorhanden

---

## Zentrale Use-Case-Kategorien

### A) Extrahieren & Transformieren

**Typische Outputs:**

- Strukturierte JSON-Extraktion
- Tabellen mit Units & Analysepopulation
- Claim-Listen mit Red Flags

**Beispiele:**

- Studienparameter extrahieren
- Text → Schema-Tabelle
- Qualitätsdokumente auf Inkonsistenzen prüfen

---

### B) Zusammenfassen & Konsolidieren

**Typische Outputs:**

- PICO-Struktur
- Ergebnistabellen mit CI/p-Werten
- Multi-Source-Konsolidierung
- Konfliktlog (nicht wegformulieren, sondern dokumentieren)

**Prinzip:**  
Narrativ folgt Tabelle – nicht umgekehrt.

---

### C) Prüfen & Bewerten (Advanced)

**Typische Outputs:**

- Rubrik-Scoring mit Evidenz
- Requirement-Matrix (`Pass` / `Partial` / `Fail` / `Unknown`)
- Gap-Analyse
- Findings Log (objektiv formuliert, keine Urteile)

**Bewertungsregel:**  
Wenn Beleg fehlt → konservativ bewerten + „Beleg fehlt“ dokumentieren.

---

## Auditierbare Output-Typen

- Evidence-annotiertes JSON
- Tabellen mit:
  - Einheit
  - Analysepopulation
  - Zeitpunkt
  - Fundstelle
- Requirement-Traceability-Matrix
- Konfliktprotokoll
- Reviewer-Findings-Log

Alle Outputs müssen so formuliert sein, dass ein Reviewer sie ohne KI nachvollziehen kann.

---

## Governance-Hinweis

- KI ist Assistenz, nicht Entscheidungsinstanz.
- Reviewer-Sign-off ist verpflichtend.
- Automatisierte Zusammenfassungen benötigen Verifier-Step.
- Keine regulatorische Freigabe ohne fachliche Prüfung.

---

## Zielsetzung Workshop 2

- Transfer von strukturiertem Prompting in wissenschaftliche Arbeitsprozesse  
- Minimierung von Halluzinations- und Compliance-Risiken  
- Aufbau reproduzierbarer, auditierbarer KI-Workflows  
- Anwendung in Studium, Forschung und regulierten Industriekontexten  
