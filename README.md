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
