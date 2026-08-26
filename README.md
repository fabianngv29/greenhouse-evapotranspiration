# Greenhouse Evapotranspiration Dataset

This repository contains the dataset used for **reference evapotranspiration (ETo) estimation under greenhouse conditions**.

The dataset includes meteorological variables directly measured by a **Davis Vantage Pro2 weather station**, variables derived by the station from the measured environmental conditions, and additional variables calculated for the estimation of reference evapotranspiration.

Data were collected under greenhouse conditions in **Juchipila, Zacatecas, Mexico**, providing a detailed characterization of both indoor and outdoor microclimatic conditions.

---

# Data

## 1. Measured Meteorological Variables

The dataset contains meteorological variables directly recorded by the monitoring system inside and outside the greenhouse.

**Variables include:**

* `Ti` → Indoor air temperature (°C)
* `To` → Outdoor air temperature (°C)
* `Hi` → Indoor relative humidity (%)
* `Ho` → Outdoor relative humidity (%)
* `Rs` → Solar radiation (W/m²)

These variables describe the main environmental conditions observed during the monitoring period.

---

## 2. Station-Derived Variables

In addition to the directly measured variables, the weather station provides several variables and environmental indices derived from the recorded meteorological conditions.

**Variables include:**

* `Di` → Indoor dew point temperature (°C)
* `Do` → Outdoor dew point temperature (°C)
* `ST` → Thermal sensation (°C)
* `IH` → Heat index (°C)
* `THSW` → Temperature-Humidity-Sun-Wind index (°C)
* `D-D` → Degree-days

These variables provide complementary information about the thermal and atmospheric conditions observed during data acquisition.

---

## 3. Reference Evapotranspiration Variables

Additional variables were calculated from the meteorological records to estimate **reference evapotranspiration (ETo)**.

The calculations follow the **FAO-56 Penman–Monteith methodology**, which considers the physical relationships among radiation, temperature, atmospheric humidity, vapor pressure, and other environmental parameters.

The dataset therefore contains the intermediate variables required for the evapotranspiration calculation, together with the resulting:

* `ETo` → Reference evapotranspiration

These calculated variables allow the complete evapotranspiration estimation process to be reproduced from the available meteorological observations.

---

# Dataset Characteristics

* **Monitoring system:** Davis Vantage Pro2
* **Environment:** Greenhouse
* **Location:** Juchipila, Zacatecas, Mexico
* **Sampling interval:** 5 min
* **Monitoring period:** July 12, 2020 to June 24, 2021
* **Number of records:** 85,989

The monitoring period includes indoor and outdoor environmental observations collected continuously, except for interruptions associated with maintenance of the monitoring system and greenhouse infrastructure.

---

## 🎯 Purpose of the Dataset

This dataset supports:

* Analysis of greenhouse microclimatic conditions
* Comparison between indoor and outdoor meteorological variables
* Analysis of directly measured and station-derived environmental variables
* Calculation of reference evapotranspiration
* Reproduction of the ETo estimation procedure
* Analysis of relationships among meteorological variables and evapotranspiration
* Development and validation of alternative evapotranspiration estimation approaches
* Reproducible research workflows

---

## 🛠 Recommended Tools

* Python + Colab / Jupyter
* Pandas
* NumPy
* Matplotlib
* SciPy

---

# Paper Related and Citation

This dataset is associated with a research article on reference evapotranspiration estimation under greenhouse conditions.

**Link to paper:** To be added after publication.

Citation information will be updated once the associated article is published.

---

## 👤 Authors

Fabián García-Vázquez
Juan Esparza-Gómez
Jesús A. Nava-Pintor
Ma. del Rosario Martínez-Blanco
Héctor A. Guerrero-Osuna
Carlos A. Olvera-Olvera
Juvenal Rodríguez-Resendiz

---

# Acknowledgements

The authors want to thank the Mexican Secretariat of Science, Humanities, Technology and Innovation (SECIHTI by its initials in Spanish) for its support to the National Laboratory of Embedded Systems, Advanced Electronics Design and Micro Systems (LN-SEDEAM by its initials in Spanish), project numbers 282357, 293384, 299061, 314841, 315947, and 321128 and scholarship number 1012274.
