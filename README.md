# Strukturiertes Prompting & Wissensaufbereitung -- Workshop Repository

![Status](https://img.shields.io/badge/status-active-blue)
![Focus](https://img.shields.io/badge/focus-regulated%20AI-critical)
![License](https://img.shields.io/badge/license-internal-lightgrey)

Repository für strukturiertes, auditierbares Prompting im Pharma- und
Behördenkontext.
Schwerpunkt: reproduzierbare Prompt-Architekturen, regulatorische
Nachvollziehbarkeit, wissenschaftliche Evidenzpflicht und Advanced-Workflows.

------------------------------------------------------------------------

## Quick Start

1.  Prinzip: **Task → Kontext → Struktur → Output-Format**
2.  Delimiter konsequent einsetzen (`<<<INPUT>>>`, XML, Markdown-Blöcke)
3.  Output explizit spezifizieren (Tabellen, JSON, strukturierte Bulletpoints)
4.  **Evidenzpflicht:** Wichtige Aussagen immer mit Zitat und Fundstelle belegen und fehlende Infos als "UNBEKANNT" zulassen.
5.  Ergebnisse fachlich validieren

------------------------------------------------------------------------

## Repository-Struktur

    .
    ├── Workshop1_Grundlagen_Prompting
    │   ├── Kernprinzipien
    │   ├── Template-Strukturen
    │   └── Regulatorische Use Cases
    │
    ├── Workshop1_Advanced_R_CustomGPT
    │   ├── Strukturierte Code-Generierung (R)
    │   ├── Validierungslogik
    │   ├── Prüfmechanismen
    │   └── CustomGPT-Workflow-Architektur
    │
    ├── Workshop2_Wissenschaftliche_Wissensaufbereitung
    │   ├── Extrahieren_Transformieren
    │   ├── Zusammenfassen_Konsolidieren
    │   └── Pruefen_Bewerten
    │
    └── README.md

------------------------------------------------------------------------

## Kerninhalte

### Workshop 1: Grundlagen -- Strukturiertes Prompting
-   Saubere Task-Definition
-   Delimiter-Architektur (Markdown/XML)
-   Output-Kontrolle
-   Fehler- und Halluzinationsreduktion
-   Einsatz im regulierten Umfeld

### Workshop 1: Advanced -- R & CustomGPT
-   Deterministische Code-Generierung
-   Eingebaute Validierungsroutinen
-   Strukturierte Analyse-Workflows
-   Governance-Design für CustomGPT-Systeme

### Workshop 2: Wissenschaftliche Wissensaufbereitung mit GenAI
-   **Zentrale Regeln:** Strikte Evidenzpflicht (Zitat + Location), Trennung von Fakt und Interpretation, sowie das Zulassen von UNBEKANNT ohne freie Erfindungen.
-   **Extrahieren & Transformieren:** Schema-first Ansatz für die Extraktion in strukturierte Formate wie JSON und Tabellen inklusive Fundstellen.
-   **Zusammenfassen & Konsolidieren:** Konsolidierung von Studien (PICO) und Erstellung von Multi-Source-Zusammenfassungen samt Konfliktlogs.
-   **Prüfen & Bewerten:** Einsatz von Rubrik-Scoring, Abgleich mit Leitlinien/DIN-Normen und Halluzinations-Guardrails durch einen dedizierten Verifier-Step.

------------------------------------------------------------------------

## Zielsetzung

-   Standardisierung von Prompt-Architekturen
-   Minimierung regulatorischer Risiken
-   Nachvollziehbare AI-Workflows (Audit Trails)
-   Transfer in Weiterbildung und Hochschulkontext

------------------------------------------------------------------------

## Governance-Hinweis

Alle generierten Inhalte sind fachlich zu prüfen.
Regulatorische Freigaben erfolgen ausschließlich durch qualifizierte
Fachstellen.
