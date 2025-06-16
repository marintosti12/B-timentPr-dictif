# 📊 Anticipation de la consommation des bâtiments non résidentiels

## 🎯 Objectif

Notre équipe s’intéresse de près à la **consommation énergétique** et aux **émissions de gaz à effet de serre** des bâtiments **non destinés à l’habitation**.

A partir de ceux déjà réalisés, vous voulez tenter de prédire les émissions de CO2 et la **consommation totale d’énergie** de bâtiments **non destinés à l’habitation**

## 🏢 Types de bâtiments étudiés

- Écoles et établissements publics (`SPS-District K-12`)
- Campus universitaires
- Bâtiments non résidentiels (`NonResidential`, `Nonresidential COS`, `Nonresidential WA`)
- Bâtiments résidentiels (`Multifamily LR`,`MultiFamily MR`,`Multifamily HR`)

## 📈 Toutes les colonnes

* OSEBuildingID                        int64
* BuildingType                        object
* PrimaryPropertyType                 object
* PropertyName                        object
* Address                             object
* ZipCode                            float64
* TaxParcelIdentificationNumber       object
* CouncilDistrictCode                  int64
* Neighborhood                        object
* Latitude                           float64
* Longitude                          float64
* YearBuilt                            int64
* NumberofBuildings                  float64
* NumberofFloors                       int64
* PropertyGFATotal                     int64
* PropertyGFAParking                   int64
* PropertyGFABuilding(s)               int64
* ListOfAllPropertyUseTypes           object
* LargestPropertyUseType              object
* LargestPropertyUseTypeGFA          float64
* SecondLargestPropertyUseType        object
* SecondLargestPropertyUseTypeGFA    float64
* ThirdLargestPropertyUseType         object
* ThirdLargestPropertyUseTypeGFA     float64
* YearsENERGYSTARCertified            object
* ENERGYSTARScore                    float64
* SiteEUI(kBtu/sf)                   float64
* SiteEUIWN(kBtu/sf)                 float64
* SourceEUI(kBtu/sf)                 float64
* SourceEUIWN(kBtu/sf)               float64
* SiteEnergyUse(kBtu)                float64
* SiteEnergyUseWN(kBtu)              float64
* SteamUse(kBtu)                     float64
* Electricity(kWh)                   float64
* Electricity(kBtu)                  float64
* NaturalGas(therms)                 float64
* NaturalGas(kBtu)                   float64
* DefaultData                           bool
* ComplianceStatus                    object
* Outlier                             object
* TotalGHGEmissions                  float64
* GHGEmissionsIntensity              float64



## 🗑️ **Colonnes à supprimer**

* OSEBuildingID = Identifiant du batiment
* PropertyName = Nom du batiment
* Address = Adresse du batiment
* TaxParcelIdentificationNumber = Numero Tax Administratif
* DefaultData = Non pertinent
* Outlier = Traitement

## 🔠 Abréviatio

**GFA** = **Gross Floor Area**

**GHG** = **Greenhouse Gas**

**EUI** = **Energy Use Intensity**


## ⚙️ Outils utilisés

- Python 3.12
- Pandas, NumPy
- Jupyter Notebook
- Poetry pour la gestion des dépendances

## 📁 Organisation du projet

- `data/` : données brutes et nettoyées
- `notebooks/` : notebooks d’exploration et de modélisation
- `src/` : code source (prétraitement, modèles, visualisation)
- `README.md` : ce fichier
- `pyproject.toml` : configuration Poetry
