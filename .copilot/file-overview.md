# Prompt Framework - Datei-Übersicht

Vollständiges Verzeichnis aller Prompt-Framework-Dateien mit Zweck und Verwendung.

---

## 📁 Dateistruktur

```
.copilot/
├── README.md                     # Hauptdokumentation & Integration-Guide
├── system-prompt.md              # Master System Prompt für Copilot
├── phase-prompts.md              # Detaillierte Prompts für alle 6 Phasen
├── conversation-patterns.md      # Konversationsmuster & Assessment
├── project-spec-template.yaml    # YAML-Template für Projekspezifikationen
├── example-project.md            # Vollständiges Beispielprojekt
└── file-overview.md              # Diese Datei
```

---

## 📄 Datei-Details

### 1. README.md
**Zweck:** Haupteinstieg und Integrations-Anleitung

**Inhalt:**
- Übersicht über das gesamte Framework
- Erklärung der 6 Lernphasen
- Adaptive Scaffolding-Strategie
- Assessment Framework Übersicht
- Engagement-Monitoring
- Conversation Patterns Zusammenfassung
- Integration in GitHub Copilot
- Beispiel-Interaktionen
- Verbindung zu Learning Paths
- Testing & Evaluation
- Anpassungs-Guidelines

**Für wen:**
- Entwickler, die das Framework integrieren
- Lehrer, die das System verstehen wollen
- Neue Nutzer als erste Anlaufstelle

**Wann verwenden:**
- Beim Setup des Systems
- Als Referenz für Gesamtübersicht
- Bei Integration in neue Projekte

---

### 2. system-prompt.md
**Zweck:** Master System Prompt - definiert Rolle und Verhalten des Copilots

**Inhalt:**
- Kernprinzipien (4 Hauptprinzipien)
  1. Adaptive Schwierigkeitsanpassung
  2. Projektbasiertes Lernen
  3. Socratic Methode & Guided Discovery
  4. Motivation & Ermutigung
- Interaktionsmuster (Projekt-Start, während Entwicklung)
- Scaffolding-Strategie (3 Level)
- Code-Vorschläge Guidelines
- Spec-Driven Development Integration
- Kommunikationsstil
- Fortschrittsverfolgung
- Best Practices (DO/DON'T)
- Technische Integration
- Beispiel-Interaktion

**Für wen:**
- GitHub Copilot (als Instruktion)
- Entwickler (um Copilot-Verhalten zu verstehen)

**Wann verwenden:**
- Als Copilot Instructions in VS Code
- Als Basis für alle Interaktionen
- Kontinuierlich aktiv während Sessions

**Integration:**
```
.github/copilot-instructions.md verweist auf diese Datei
oder:
VS Code Settings → Copilot Instructions → Inhalt dieser Datei
```

---

### 3. phase-prompts.md
**Zweck:** Detaillierte, verwendbare Prompts für alle 6 Lernphasen

**Inhalt:**

#### Phase 1: Projektinitiierung
- Eröffnungs-Prompts
- Vertiefungs-Fragen (3 Level-Varianten)
- Lernziel-Identifikation
- Motivations-Verstärkung

#### Phase 2: Exploration & Anforderungsanalyse
- Anforderungs-Dialog
- Iterative Verfeinerung
- Spec-Generierung (automatisch)
- Bestätigungs-Prompt

#### Phase 3: Konzept & Design
- Design-Einführung (3 Level-Varianten)
- Modellierungs-Hilfen
- Design-Review-Fragen

#### Phase 4: Implementation
- Implementierungs-Start (3 Level-Varianten)
- Scaffolding während Implementation
- Progressiver Hinweis-Mechanismus (4 Stufen)
- Code-Review & Feedback

#### Phase 5: Reflexion & Debugging
- Debugging-Strategien (3 Level-Varianten)
- Reflexions-Prompts
- Code-Review Session
- Metacognitive Questions

#### Phase 6: Dokumentation & Präsentation
- Dokumentations-Anleitung
- Dev-Log erstellen (3 Level-Varianten)
- Präsentations-Vorbereitung
- Code-Kommentierung

#### Zusätzlich:
- Zusammenfassung & Abschluss
- Meta-Prompts (für Copilot-Selbstreflexion)

**Für wen:**
- Copilot (als Prompt-Vorlagen)
- Entwickler (zum Verstehen der Phasen)
- Lehrer (als didaktische Referenz)

**Wann verwenden:**
- Copilot wählt automatisch passende Phase
- Bei Projekt-Start: Phase 1
- Bei Implementation: Phase 4
- Bei Fehler: Phase 5
- Etc.

**Format:**
Jeder Prompt ist kopierbar und direkt verwendbar, mit Platzhaltern:
```
[PROJEKT-TYP], [Lernziel 1], [PROJEKT-NAME], etc.
```

---

### 4. conversation-patterns.md
**Zweck:** Framework für Konversation, Assessment und adaptive Anpassung

**Inhalt:**

#### Teil 1: Conversation Patterns
- **Frage-Typen:**
  - Open-Ended Questions
  - Guided Discovery Questions
  - Socratic Questions
  - Checkpoint Questions
  
- **Feedback-Patterns:**
  - Positive Reinforcement
  - Constructive Feedback
  - Scaffolded Hints (4 Stufen)

- **Conversation Flows:**
  - Neue Konzept-Einführung
  - Debugging Session
  - Code Review

#### Teil 2: Assessment Framework
- **Wissensstand-Assessment:**
  - Automatische Indikator-Erkennung
  - Assessment-Algorithmus (Python Pseudo-Code)

- **Lernfortschritt-Tracking:**
  - Konzept-Mastery Matrix (6 Stufen)
  - Progress-Metriken (quantitativ & qualitativ)

- **Adaptive Scaffolding:**
  - Scaffolding-Levels (high/medium/low)
  - Fading-Strategy
  - Zone of Proximal Development (ZPD) Mapping

- **Engagement & Motivation Tracking:**
  - Engagement-Indikatoren
  - Motivation-Strategien (intrinsic/extrinsic)
  - Amotivation-Prevention

#### Teil 3: Implementierungs-Guidelines
- Copilot Decision Tree
- Adaptive Behavior Algorithm (Python Pseudo-Code)

**Für wen:**
- Entwickler (Implementation-Details)
- Copilot (Decision-Making Logic)
- Forscher (Didaktische Theorie)

**Wann verwenden:**
- Bei Entwicklung von Copilot-Logik
- Für Assessment-System-Implementation
- Als Referenz für Conversation-Entscheidungen

**Besonderheit:**
Enthält ausführbare Logik (Pseudo-Code) für automatisierte Entscheidungen.

---

### 5. project-spec-template.yaml
**Zweck:** Strukturiertes Template für Projekt-Spezifikationen

**Inhalt:**

#### Hauptsektionen:
1. **Projektinformationen**
   - Name, Typ, Beschreibung
   - Technologie-Stack
   - Repository-Info
   - Dateistruktur

2. **Ziele & Erfolg**
   - Hauptziel, Teilziele
   - Success Criteria
   - MVP-Definition

3. **Anforderungen**
   - Funktionale Requirements
   - Nicht-funktionale Requirements
   - Interaktionen (Inputs/Outputs)

4. **Lernziele**
   - Pro Konzept: ID, Titel, Beschreibung
   - Level, Kategorie, Status
   - Verwendung im Code
   - Ressourcen & Checkpoints

5. **Meilensteine**
   - Pro Meilenstein: Titel, Tasks
   - Status, Deliverables
   - Learning Focus

6. **Student-Profil**
   - Level, bekannte Konzepte
   - Lerngeschwindigkeit
   - Präferenzen
   - Fortschritt & Statistiken
   - Engagement-Tracking

7. **Reflexion & Learnings**
   - Dev-Logs
   - Gelernte Konzepte
   - Häufige Fehler

8. **Assessment & Evaluation**
   - Automatische Checks
   - Selbst-Assessment
   - Copilot-Assessment

9. **Nächste Schritte**
   - Immediate Actions
   - Future Projects
   - Recommended Resources

10. **Metadaten & Tracking**
    - Versions-Info
    - Changelog
    - Tags, Status

**Für wen:**
- Copilot (erstellt automatisch project-spec.yaml)
- Schüler (sieht Fortschritt und Ziele)
- Lehrer (monitort Lernfortschritt)

**Wann verwenden:**
- Bei Projekt-Start: Automatische Generierung
- Während Projekt: Kontinuierliche Updates
- Nach Abschluss: Als Lern-Dokumentation

**Format:**
Standard YAML mit ausführlichen Kommentaren für Verständlichkeit.

**Output:**
Jedes Projekt bekommt eigene `.copilot/project-spec.yaml` Datei.

---

### 6. example-project.md
**Zweck:** Vollständiges Durchlauf-Beispiel eines Lernprojekts

**Inhalt:**

#### Projekt: Zahlen-Ratespiel
- **Vollständige project-spec.yaml** (ausgefüllt)
- **Finaler Code** (kommentiert)
- **Lernreise-Dokumentation** durch alle 6 Phasen:
  1. Projektinitiierung (Dialog)
  2. Anforderungen klären (Dialog)
  3. Design & Modellierung (Dialog)
  4. Implementation (6 Schritte mit Dialogen)
  5. Reflexion (Dialog)
  6. Dokumentation (Code-Kommentare)

#### Zusätzlich:
- **Lessons Learned** (Was gut funktioniert hat)
- **Adaptionen während Projekt** (Engagement, Verständnis-Checks)
- **Success-Tracking**
- **Verwendung als Template** (Variationen für verschiedene Level)

**Für wen:**
- Neue Nutzer (zeigt kompletten Ablauf)
- Entwickler (Template für Tests)
- Lehrer (Beispiel für didaktischen Einsatz)

**Wann verwenden:**
- Als Inspiration für neue Projekte
- Zum Testen des Frameworks
- Als Demonstration des vollständigen Workflows

**Besonderheit:**
Enthält **echte Dialoge** zwischen Copilot und fiktivem Schüler "Max", 
zeigt adaptive Anpassungen in Echtzeit.

---

## 🔄 Zusammenspiel der Dateien

```
┌─────────────────────────────────────────────────────────────┐
│                       README.md                             │
│        (Einstiegspunkt, Übersicht, Integration)            │
└────────────────────────┬────────────────────────────────────┘
                         │
         ┌───────────────┼───────────────┐
         │               │               │
         ▼               ▼               ▼
┌────────────────┐ ┌────────────┐ ┌──────────────┐
│ system-prompt  │ │  phase-    │ │ conversation-│
│     .md        │ │ prompts.md │ │  patterns.md │
│ (Rolle & Core) │ │ (6 Phasen) │ │ (Assessment) │
└────────┬───────┘ └─────┬──────┘ └──────┬───────┘
         │               │               │
         │       ┌───────┴───────┐       │
         │       │               │       │
         ▼       ▼               ▼       ▼
    ┌────────────────────────────────────────┐
    │  GitHub Copilot (Adaptive AI Tutor)    │
    │  - Liest alle Dateien                  │
    │  - Wählt passende Prompts              │
    │  - Generiert Responses                 │
    │  - Tracked Progress                    │
    └────────────┬───────────────────────────┘
                 │
                 │ erstellt/aktualisiert
                 │
                 ▼
    ┌────────────────────────────┐
    │ project-spec-template.yaml │
    │ → project-spec.yaml        │
    │   (für jedes Projekt)      │
    └────────────┬───────────────┘
                 │
                 │ Beispiel
                 │
                 ▼
    ┌────────────────────────────┐
    │   example-project.md       │
    │   (Zahlen-Ratespiel)       │
    │   - Zeigt vollständigen    │
    │     Workflow               │
    └────────────────────────────┘
```

---

## 🎯 Verwendungsszenarien

### Szenario 1: Neuer Schüler startet erstes Projekt

**Ablauf:**
1. Copilot liest `system-prompt.md` (Rolle verstehen)
2. Copilot nutzt `phase-prompts.md` → **Phase 1** (Projektinitiierung)
3. Dialog mit Schüler (offene Fragen)
4. Copilot nutzt `conversation-patterns.md` → Assessment (Level erkennen)
5. Copilot erstellt `project-spec.yaml` basierend auf `project-spec-template.yaml`
6. Weiter durch Phase 2-6 mit passenden Prompts
7. Kontinuierliches Update von `project-spec.yaml`

**Verwendete Dateien:**
- `system-prompt.md` ✅ (Verhalten)
- `phase-prompts.md` ✅ (Dialoge)
- `conversation-patterns.md` ✅ (Assessment)
- `project-spec-template.yaml` ✅ (Struktur)

---

### Szenario 2: Schüler hat Fehler im Code (Debugging)

**Ablauf:**
1. Copilot erkennt Fehler-Situation
2. Copilot nutzt `conversation-patterns.md` → Decision Tree → "Error-Handling"
3. Copilot nutzt `phase-prompts.md` → **Phase 5** (Debugging)
4. Assessment: Welcher Error-Type? (Syntax/Logic/Conceptual)
5. Passende Debugging-Strategie wählen (Level-abhängig)
6. Guided Debugging Session
7. Update `project-spec.yaml` → common_mistakes Sektion

**Verwendete Dateien:**
- `conversation-patterns.md` ✅ (Decision Tree, Error-Handling)
- `phase-prompts.md` ✅ (Phase 5 Debugging)
- `project-spec.yaml` ✅ (Tracking)

---

### Szenario 3: Entwickler integriert Framework in neues System

**Ablauf:**
1. Liest `README.md` (Übersicht)
2. Versteht `system-prompt.md` (Copilot-Verhalten)
3. Implementiert Logic aus `conversation-patterns.md` (Decision Tree, Assessment)
4. Konfiguriert Copilot mit Instructions
5. Testet mit `example-project.md` (Beispiel durchspielen)
6. Passt Prompts an eigene Bedürfnisse an

**Verwendete Dateien:**
- `README.md` ✅ (Integration-Guide)
- `system-prompt.md` ✅ (Core Behavior)
- `conversation-patterns.md` ✅ (Implementation)
- `example-project.md` ✅ (Testing)

---

## 📊 Datei-Größen & Komplexität

| Datei | Zeilen | Komplexität | Verwendung |
|-------|--------|-------------|------------|
| `README.md` | ~450 | Mittel | Dokumentation |
| `system-prompt.md` | ~250 | Niedrig | Copilot Instructions |
| `phase-prompts.md` | ~1200 | Hoch | Prompt-Bibliothek |
| `conversation-patterns.md` | ~900 | Sehr Hoch | Logic & Assessment |
| `project-spec-template.yaml` | ~450 | Mittel | Data Structure |
| `example-project.md` | ~750 | Niedrig | Demonstration |
| **TOTAL** | **~4000** | - | Komplettes Framework |

---

## 🔧 Anpassung & Erweiterung

### Neue Prompts hinzufügen

**Datei:** `phase-prompts.md`

**Vorgehen:**
1. Identifiziere Phase und Level
2. Füge neuen Prompt im entsprechenden Abschnitt ein
3. Folge dem Format der existierenden Prompts
4. Teste mit Beispiel-Projekt

### Neues Konzept zum Assessment hinzufügen

**Datei:** `conversation-patterns.md` → Teil 2 → Concept-Mastery Matrix

**Vorgehen:**
1. Definiere 6 Mastery-Stages für Konzept
2. Lege Assessment-Methoden fest
3. Definiere Mastery-Criteria
4. Füge zu `project-spec-template.yaml` → learning_objectives hinzu

### Neue Programmiersprache unterstützen

**Dateien:** `phase-prompts.md` + `project-spec-template.yaml`

**Vorgehen:**
1. Passe Code-Beispiele in `phase-prompts.md` an
2. Füge sprachspezifische Patterns hinzu
3. Erweitere `technology` Sektion in YAML-Template
4. Erstelle sprachspezifisches Beispiel-Projekt

---

## 📚 Lern-Ressourcen-Integration

Das Framework ist designed, um mit den **Learning Paths** zu arbeiten:

```
Verbindung:
learning-paths/*.md  →  Konzept-Details & Übungen
            ↕
.copilot/phase-prompts.md  →  Verweise auf Learning Paths
            ↕
project-spec.yaml  →  learning_objectives.resources
```

**Beispiel:**
```yaml
learning_objectives:
  - concept: "oop"
    resources:
      - type: "learning-path"
        path: "/learning-paths/object-oriented-software-construction.md"
        section: "Module 2: Classes & Objects"
```

Copilot kann dann sagen:
```
"Super! Du verstehst jetzt Klassen! 🎉
Wenn du tiefer in OOP einsteigen willst, schau dir 
'Object-Oriented Software Construction' in den Learning Paths an!"
```

---

## 🧪 Testing-Strategie

### Unit-Tests (für einzelne Komponenten)

**Test:** Phase 1 Prompts
- Input: Anfänger-Schüler, Spiel-Projekt
- Expected: Open-Ended Questions, High Scaffolding
- Verify: Prompt-Format, Ton, Komplexität

**Test:** Assessment-Algorithmus
- Input: Code-Sample, Frage-Historie
- Expected: Korrektes Level (Beginner/Intermediate/Advanced)
- Verify: Score-Berechnung

### Integration-Tests (vollständiger Workflow)

**Test:** Komplettes Projekt (wie example-project.md)
- Start: Phase 1 (Ideenfindung)
- Through: Alle 6 Phasen
- End: Dokumentiertes, funktionierendes Projekt
- Verify: Spec-File vollständig, Code läuft, Lernziele erreicht

### A/B-Tests (Optimierung)

**Test:** Scaffolding-Levels
- Variant A: High Scaffolding
- Variant B: Medium Scaffolding
- Measure: Time to mastery, Engagement, Satisfaction

---

## 🚀 Deployment-Checkliste

Bei Integration in Production:

- [ ] Alle Dateien im `.copilot/` Verzeichnis vorhanden
- [ ] `system-prompt.md` als Copilot Instruction konfiguriert
- [ ] `project-spec-template.yaml` validiert (gültige YAML-Syntax)
- [ ] Prompts auf Zielgruppe angepasst (Alter, Sprache, Vorkenntnisse)
- [ ] Beispiel-Projekt getestet (funktioniert Workflow?)
- [ ] Learning Paths verlinkt (falls vorhanden)
- [ ] Monitoring aktiv (Track Engagement, Lernfortschritt)
- [ ] Feedback-Loop eingerichtet (Verbesserungen sammeln)

---

## 📖 Weitere Dokumentation

Für tiefere Einblicke siehe auch:

- **Theoretische Grundlagen:** `README.md` → "Weitere Ressourcen"
- **Didaktik-Literatur:** `README.md` → "Didaktik-Literatur"
- **Implementation-Details:** `conversation-patterns.md` → Teil 3
- **YAML-Spec Details:** `project-spec-template.yaml` (ausführliche Kommentare)

---

**Framework-Version:** 1.0  
**Letzte Aktualisierung:** März 2025  
**Maintainer:** Projekt-Team "project-based-learning"

---

**Happy Coding & Teaching! 🚀**
