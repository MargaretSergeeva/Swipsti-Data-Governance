# Swipsti Brauerei – Data-Governance-Strategie & Pilot

**Abschlussprojekt · Beam Institute of Technology (Billigence Data Academy), 2025**
Team: Dorcas Iradukunda, Mckinley Black, Margarita Sergeeva – ein internationales Team mit unterschiedlichen fachlichen Hintergründen.

Präsentationen:(https://margaretsergeeva.github.io/swipsti-data-governance/)

## Ausgangslage

Swipsti ist eine Craft-Brauerei mit 250 Mitarbeitenden, die bundesweit über Handel, Gastronomie und einen Online-Shop verkauft. Die Organisation war noch von der Start-up-Phase geprägt und nicht auf Wachstum ausgerichtet. Ziel des Managements: die Organisation skalieren und den Online-Shop für mehr Cross-Selling ausbauen.

Die Interviews mit dem Management zeigten:

- **Datensilos:** MES, LIMS, ERP, CRM und Logistiksoftware arbeiteten getrennt – ohne zentrales Data Warehouse oder Data Catalog.
- **Keine Verantwortlichkeiten:** Es gab keine Data Owner oder Data Stewards; die IT verantwortete die Systeme, nicht die Inhalte.
- **Keine gemeinsame Sprache:** „Ausstoß“, „Kunde“ oder „Charge“ bedeuteten in Controlling, Produktion und Vertrieb jeweils etwas anderes.
- **Dezentrales Reporting:** Jede Abteilung baute eigene Power-BI-Dashboards; KPIs wurden manuell und oft verspätet konsolidiert.
- **Compliance-Lücken:** Eine externe Datenschutzbeauftragte, aber kein internes Monitoring und kein DSGVO-Verarbeitungsverzeichnis.
- **KI-Ideen ohne Fundament:** Absatzprognose und „Predictive Brewing“ waren angedacht – Strategie, Know-how und Governance fehlten.

## Teil I – Assessment & Strategie

1. **Ist-Analyse mit dem DX Framework** – vollständige Bewertung über alle Data-Excellence-Elemente (Daten planen, verantworten, strukturieren, schützen, nutzen, nachvollziehen, optimieren): **Reifegrad 2,55 von 5**.
2. **Maßnahmenpriorisierung nach Aufwand & Wirkung** – Quick Wins (Rollen, Fachdatenmodell, Datenkatalog, Datenkompetenz), strategische Ziele (Richtlinien & Standards, MDMS, zentrale Datenplattform, KI & Analytics), Effizienzreserven und Zukunftsinvestitionen.
3. **Data Excellence Roadmap** – von Rollen und Business Glossary über Richtlinien und Metadatenmanagement bis zur zentralen Datenplattform und ersten KI-Piloten.
4. **Data-Governance-Organisation** – DX Center und Gremien auf drei Ebenen (Direct / Control / Execute), Rollen wie Data Owner, Data Steward, Data Architect, Metadata Manager und DX Demand Manager – nach dem Prinzip „mehrere Hüte auf einem Kopf“ statt neuer Stellen.
5. **Prozesse & RACI** – tägliche, wöchentliche und monatliche Governance-Prozesse, ein Anforderungsprozess für Data Consumer/Producer mit RACI-Matrix sowie operative und außergewöhnliche Eskalationspfade.
6. **Harmonisierung zentraler Begriffe** – Fachdatenmodell top-down (Prinzipien, Begriffe, Verantwortlichkeiten) und bottom-up (tatsächliche Datennutzung, Kennzahlen, Konflikte), dokumentiert im Business Glossary.

## Teil II – Implementierung & Pilot

1. **Tool-Auswahl** – Dataspot, Collibra und Informatica anhand von 10 Kriterien bewertet; Entscheidung für **Dataspot** (Rollenmanagement, Usability, Katalog & Glossar, geringste Kosten).
2. **Pilotauswahl & Scope** – Pilot **Vertrieb & Online-Shop**: motiviertes Team, klar abgegrenzte Domäne, höchster strategischer Nutzen und messbarer ROI. Scope über Business-Capabilities-Analyse und eine Process-Data-Matrix für den Online-Bestellprozess.
3. **Stakeholder-Analyse** – CEO, CFO, Vertriebsmanagement und Vertriebsmitarbeitende mit Interessen und Einfluss.
4. **Regulatorik & Standards** – DSGVO, PCI DSS und EU AI Act bewertet; interne Standards für Begriffe, Namenskonventionen, Klassifizierung, Data-Quality-Checks und rollenbasierte Zugriffe.
5. **Tech-Stack** – Bestandsaufnahme der Systeme: AWS, Salesforce (CRM), SAP (ERP), Shopify (E-Commerce), Mulesoft, S3 Data Lake, PostgreSQL, Tableau.
6. **Datenmodellierung** – erst das **Fachdatenmodell**, dann das **technische Datenmodell** mit Datentypen und -formaten, modelliert in Dataspot.
7. **Data Warehouse** – **PostgreSQL-Datenbank im Star-Schema**, befüllt mit synthetischen Daten, inklusive End-to-End Data Lineage.
8. **Dashboards** – Marketing- und Management-Dashboards in **Tableau** (Kunden, Bestellungen, Kampagnen) sowie Data-Quality-KPIs.
9. **Change Management** – Datenkultur, Data Literacy und das ADKAR-Modell sowie ein kontinuierlicher Verbesserungsprozess (KVP) mit KPIs in Dataspot.

## Ergebnis

- **Reifegrad:** Zielwert von 2,55 auf **3,65 von 5** – stabile Governance, dokumentierte Datenflüsse und erste Qualitätsregeln.
- **Governance:** einheitliches Business-Glossar, klare Rollen und Verantwortlichkeiten, zentral definierte KPIs.
- **Integrierte Datenplattform:** ERP, CRM, Webshop und Amazon (SP-API) fließen in einen Data Lake auf AWS; per EL-Prozess in ein PostgreSQL-Data-Warehouse als kanalübergreifende Single Source of Truth. Bereinigte Daten werden per Reverse Sync an ERP und CRM zurückgespielt.
- **Reporting:** Tableau direkt an das PostgreSQL-DWH angebunden – zentrale Dashboards statt getrennter Abteilungsberichte.
- **KI-Readiness:** eine gesteuerte Datenbasis für das erste KI-Pilotprojekt.
