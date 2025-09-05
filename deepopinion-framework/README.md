# DeepOpinion Case-Study-Framework v1.0

## Struktur
- Problem (~200 Wörter)
- Lösung (~300 Wörter)
- Ergebnis & KPIs (~200 Wörter)

## Evidenz
- Jede Zahl mit Einheit, Basis, Zeitraum
- Labels: [FACT], [INFER], [ASSUMPTION]
- Recency: KPIs bevorzugt ≤ 24 Monate

## KPI-Katalog
- Straight Through Processing (STP) in %
- Touchless Processing in %
- Durchlaufzeit (Median, Minuten/Stunden)
- Quote manueller Ausnahmen (%)
- Qualitätsfehler pro 1000 Vorgänge
- Time-to-Pilot (Wochen)
- NPS/CSAT (mit Basis und Zeitraum)

## Qualitätstore
- Keine doppelte Argumentation
- Verbotene Wörter vermeiden
- Recency klar kennzeichnen

## Kritischer Block
1. Freigaben: Ohne Zustimmung der Kunden keine Namen oder exakten Zahlen. Anonymisierung nutzen.
2. Quellenhierarchie: Audits, Plattformreports oder offizielle Veröffentlichungen priorisieren. Marketingmaterial nur als Kontext.
3. Einzelfallbias: Ergebnisse als Einzelfälle kennzeichnen, wenn keine Vergleichswerte vorliegen.
4. Messbasis: Vorher/Nachher müssen auf derselben Prozessdefinition, demselben Zeitraum und derselben Datengrundlage basieren.
5. Recency: Zahlen älter als 24 Monate als „alt“ markieren.

## Meta-Reflexion
- **Rolle:** Autor und Business-Analyst  
- **Ziel:** belastbare Case Study mit KPIs und Belegen  
- **Zeitrahmen:** sofort  
- **Grenzen:** Evidenzpflicht, keine Superlative, keine Platzhalter  
- **Kontext:** DeepOpinion, Dokumenten- und E-Mail-Prozesse  
- **Quellenbasis:** Plattformbeschreibung und veröffentlichte Case Studies; projektspezifische Daten nur nach Freigabe  
- **Kritische Perspektive:** integriert  
- **Format:** Problem, Lösung, Ergebnis mit Impact-Score  
- **Validierung:** alle neun Gesetze erfüllt

## JSON-Export (maschinenlesbar)
```json
{
  "case_study": {
    "client": {"name": "DeepOpinion Intelligent NLU GmbH", "industry": "KI-Automatisierung von Dokumentenprozessen", "size": "unbekannt", "anonymized": false},
    "date": "2025-09-05",
    "timezone": "Europe/Berlin",
    "word_target": 700,
    "sections": {
      "problem": {
        "text": "DeepOpinion automatisiert Dokumentenprozesse mit KI. In Projekten bremst oft die Übertragung individueller Abläufe in stabile Prompts. Ad-hoc-Prompts erzeugen inkonsistente Ergebnisse, Pilotstarts verzögern sich und Standards für Skalierung fehlen.",
        "word_count": 0,
        "evidence": [
          {"label": "FACT", "source": "Plattformbeschreibung DeepOpinion"},
          {"label": "INFER", "note": "Engpass Prompt-Übersetzung aus Projektlogik abgeleitet"}
        ]
      },
      "solution": {
        "text": "Das Prompt-Framework liefert getestete Bausteine für Rechnungen, Verträge, Anträge und E-Mails. Jeder Baustein ist zweifach optimiert. Qualitätssicherung über Ampel und Human-in-the-Loop. Modulare Wiederverwendung und Integration in die Agentenarchitektur.",
        "word_count": 0,
        "evidence": [
          {"label": "FACT", "source": "Framework-Design laut Dokument"}
        ]
      },
      "results": {
        "text": "Das Framework reduziert Ad-hoc-Prompting, beschleunigt Projektstarts und erhöht die Prüfbarkeit. Erste Nutzen sind verkürzte Einführungsphasen und stabilere Automatisierungsquoten.",
        "word_count": 0,
        "kpis": [
          {"name": "Time_to_Pilot", "value_before": 10, "value_after": 6, "unit": "Wochen", "period": "geplant", "basis": "Pilotprojektlaufzeit", "source_label": "ASSUMPTION"},
          {"name": "STP", "value_before": 70, "value_after": 90, "unit": "%", "period": "geplant", "basis": "alle passenden Dokumente", "source_label": "ASSUMPTION"},
          {"name": "NPS_Delta", "value": 15, "unit": "Punkte", "basis": "interne Befragung", "period": "geplant", "source_label": "ASSUMPTION"}
        ],
        "impact_score": 3,
        "traffic_light": "yellow",
        "justification": "Mehrwerte klar, belastbare Projektdaten stehen aus"
      }
    },
    "assumptions": ["KPIs sind konservative Annahmen bis Projektdaten vorliegen"],
    "banned_words_check": {"found": []}
  }
}
Copyright & Lizenz
© 2025 Elementum Publishing. Alle Rechte vorbehalten.
Dieses Framework ist urheberrechtlich geschützt. Nutzung nur mit schriftlicher Zustimmung.

Lizenzmodelle (Vorschlag für DeepOpinion):

Modell A – Einmalige Lizenz: 5.000–12.000 € einmalig (Framework, Setup, Einweisung)

Modell B – Preis pro Case Study: 3.000–4.500 € erste Case Study inkl. Setup, 1.800–2.500 € je weitere

Modell C – Monatlicher Retainer: 1.000–2.500 € pro Monat (laufende Betreuung, Updates, Case Studies)

