- Sind Data Warehouse und Data Integration zwei verschiedene Konzepte oder gehören die zueinander?
- David nach Kernarbeitszeiten fragen

## Data Warehouse
- Daten werden vor dem Einlagern formatiert

## Data Lake
- Unsortierte unformatierte Daten, müssen vor Abfrage formatiert werden

## Data Mart
- Data Warehouse formatiert in einzelne Marts (finance, personal, etc.)


## Data Vault
- Source -> Staging Area -> Core(Raw Vault - Business Vault) -> Raw-/Information Marts
- -> heißt ETL (Extract, Transform, Load)
- Im Core werden aus den Daten automatisch weitere Daten generiert (Bestellungen automatisiert je nach Situation (Jahreszeit etc.))
- Moderne Version des Warehouses
- Bessere Anpassung an Befürfnisse des Unternehmens
- 