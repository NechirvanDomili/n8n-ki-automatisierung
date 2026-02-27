# Präsentation: n8n & KI – Intelligente Automatisierung

**Autor:** Nechirvan Haso Sodo Domili  
**Datum:** 01.12.2025

## 1. Was ist n8n?

- Visuelle Automations-Plattform (node-basiert)
- Fair-Code Workflow Automation
- Verbindet APIs, Datenbanken, Webhooks und SaaS-Systeme
- Flows nach dem Muster: **Trigger → Verarbeitung → Aktion**

n8n wurde Ende 2019 von Jannik Beyerstedt in Berlin gegründet und hat sich seitdem als starkes Integrations- und Automatisierungswerkzeug etabliert.

## 2. Warum n8n?

### Flexibilität in der Implementierung

- Self-Hosted
- Cloud

### Kernkonzept

- **Nodes:** Funktionsblöcke (z. B. Trigger, HTTP, Code, AI)
- **Workflow:** Verknüpfung der Nodes zu einem End-to-End-Prozess
- **Visuelle Konfiguration:** Schnellere Entwicklung als rein skriptbasierte API-Orchestrierung

## 3. Wie funktioniert n8n?

### Typische Trigger

- **Manual Trigger:** Für Tests/Debugging
- **Schedule Trigger:** Zeitgesteuert per Cron
- **Tool-spezifische Trigger:** z. B. Typeform/Salesforce/Webhooks

### Kontrollierter Datenfluss

- Daten laufen Schritt für Schritt durch den Workflow
- Branching via IF/Switch
- Fehlerbehandlung via Error Workflows

### Power Nodes

- **Code Node:** Eigene Logik in JavaScript
- **HTTP Request Node:** Flexible API-Anbindung

## 4. KI mit n8n

### KI-Module in n8n

- AI- und LangChain-Nodes
- Einsatz für Generierung, Analyse, Klassifikation und Extraktion
- Standard-Nodes als Tools für Agenten nutzbar

### Typische KI-Bausteine

- **LLM Nodes** (z. B. OpenAI, Anthropic)
- **Prompt/Chain Nodes** für mehrstufige Logik
- **Memory Nodes** für Kontext über mehrere Schritte
- **Embeddings & Vector Stores** für semantische Suche und RAG

## 5. Praxisbeispiele

### A) RAG-Bot

- User-Anfrage wird eingebettet
- Ähnliche Inhalte im Vector Store gesucht
- LLM erstellt Antwort mit Kontext
- Optional: Memory für Multi-Turn-Gespräche

### B) Automatische Case-Datenzuordnung in Salesforce

- Trigger bei neuen/aktualisierten Cases
- Dokumente laden und extrahieren
- KI-Agent ordnet Daten/Attribute zu
- Ergebnisse in Salesforce zurückschreiben
- Fehlerfälle in Error-Workflow mit Notification

## 6. Advanced Features: KI und Robustheit

- KI-Integration mit OpenAI
- System Prompt definieren
- Daten-Injektion für Personalisierung
- Error Workflow für Robustheit
- Sofortige Error Notifications

## 7. Best Practices

- Prompt klar strukturieren (Rolle, Ziel, Format, Beispiele)
- Guardrails durch Parsing/Validierung (z. B. JSON-Schema)
- Human-in-the-Loop vor kritischen Aktionen
- Kosten/Latenz optimieren (kleinere Modelle, Caching)
- Logging und Evaluierung zur kontinuierlichen Verbesserung

## 8. Fazit & Next Steps

- n8n ist ein praktischer Orchestrator für KI-gestützte Prozessautomatisierung
- Besonders wirksam durch Kombination aus Integrationen, Logik und Governance
- Nächste Schritte:
  - Produktive Pilot-Workflows auswählen
  - Monitoring/Alerting standardisieren
  - Prompts und Modelle iterativ verbessern
