# Prompt-Extraktor v2.2

...

## Ausgabeformate

### Markdown pro Prompt
- ID: PR-01  
- Prompttext: vollständiger Prompttext  
- Status: neu \| aktualisiert \| unverändert (nur bei mode=delta)  
- Stärken: 1–2 Sätze  
- Einsatzfelder: 1–2 Sätze  
- Lite-Version: kurze Variante  

### JSON Sammlung (Beispiel)

```json
{
  "meta": {
    "run_id": "2025-08-13T00:00:00Z-ABC123",
    "previous_run_id": null,
    "model": "gpt-5-thinking"
  },
  "prompts": [
    {
      "id": "PR-01",
      "prompt": "Analysiere einen gegebenen Text und extrahiere drei Kernthemen.",
      "status": "neu"
    }
  ]
}
Fehler und Abbruchlogik
No-Go: keine gültigen Kerne → gib nur eine knappe Begründung aus, ohne Sammlung.

Go: mindestens ein Kern → liefere exakt die gewählten Ausgaben.

Budget/Timebox erreicht: liefere Kopfhinweis plus Teilergebnis.

Option: eingebaute Mini-Selftests
selftest=true führt zwei Checks aus:

Negativtest: künstliches Log ohne validen Kern → erwarteter Abbruch.

Dedup-Test: zwei nahezu gleiche Kandidaten → erwartetes Merge bei Jaccard ≥ 0.60.

Ergebnis vor der regulären Ausgabe als Kurzblock.
