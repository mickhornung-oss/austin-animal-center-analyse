# Austin Animal Center – Datenanalyse & Modellierung

End-to-End Datenmodellierung und explorative Analyse von über 79.000 Tierheim-Datensätzen des Austin Animal Center (2013–2018).

## Projektziel
Aus einem flachen, unstrukturierten Rohdatensatz wurde ein relationales Datenmodell (Sternschema) aufgebaut und daraus Business-Insights zur Prozessoptimierung und Kapazitätsplanung abgeleitet.

## Architektur & Modell
- **Faktentabelle:** Alle Ereignisse (Intakes, Outcomes, Adoptionen, Euthanasien)
- **Dimensionstabellen:** `dim_animal` (Tier-Metadaten) und `dim_date` (Zeitliche Einordnung)

## Kernerkenntnisse
* **Saisonalität:** Die Adoptionsrate folgt einem klaren Rhythmus (Anstieg im Sommer, Rückgang im Winter).
* **Prozess-Engpässe:** 88% der Tiere kommen gesund an. Dennoch müssen auch gesunde Tiere euthanasiert werden (4% der Euthanasien) – ein Kapazitätsproblem, kein Aufnahmeproblem.
* **Erfolgsmessung:** Die Euthanasiequote sank kontinuierlich von über 10% auf unter 8%.

## Tech Stack
* Python · pandas · matplotlib · Datenmodellierung (Sternschema)

## Lokale Ausführung
1. Repository klonen
2. `pip install pandas matplotlib`
3. Jupyter Notebook öffnen und ausführen
