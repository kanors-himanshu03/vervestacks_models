# JPN — VerveStacks ESOM Model

!!! info "Model Run"
    **Generated:** 2026-05-13 17:01:00  |  **ISO Code:** `JPN`

---

## Model Calibration 2022

| **Total Capacity** | **Total Generation** | **CO2 Emissions** | **Calibration to EMBER** |
|--------------|---------------|------------|--------------------------|
| 325 GW | 1041 TWh | 536 Mt | 99% |

> **Note:** 2022 fossil and bio capacity is calibrated to EMBER and renewable capacities to IRENA.
> UNSD has incomplete data for fuel consumption, so calibration is demonstrated against total CO₂ emissions
> reported by EMBER — confirming that efficiency assumptions are sound.

---

## Power Generation Assets

### Existing Capacity

| **Fuel Type** | **Threshold** | **Plants Above Threshold** | **Active Capacity** | **Mothballed Capacity** | **Wtd Avg Efficiency** |
|---------------|---------------|----------------------------|--------------------|--------------------------|-----------------|
| 🌱 **Bioenergy** | 50 MW | 70/129 plants | 6.64 GW | 0.075 GW | 28.4% |
| ⚫ **Coal** | 490 MW | 58/174 plants | 55 GW | 1.08 GW | 35.3% |
| 🔥 **Gas** | 490 MW | 91/168 plants | 89 GW | — | 44.4% |
| 🌋 **Geothermal** | 60 MW | 1/30 plants | 0.669 GW | — | 100% |
| 💧 **Hydro Power** | 60 MW | 111/164 plants | 26.5 GW | — | 70% |
| ⚛️ **Nuclear** | — | 35/35 plants | 14.4 GW | 21.5 GW | 100% |
| 🛢️ **Oil** | 490 MW | 10/29 plants | 9.86 GW | 1.15 GW | 29.2% |
| ☀️ **Solar** | 200 MW | 56/306 plants | 88 GW | — | 59% |
| 🌊 **Windoff** | 200 MW | 2/11 plants | 1.73 GW | — | 97% |
| 💨 **Windon** | 200 MW | 4/129 plants | 5.73 GW | — | 92% |
| 🔋 **Pumped Storage** | 60 MW | 34/35 plants | 23.7 GW | — | 100% |


### Future Projects (offered for endogenous selection)

| **Fuel Type** | **Threshold** | **Plants Above Threshold** | **Total Capacity** | **Wtd Avg Efficiency** |
|---------------|---------------|----------------------------|--------------------|-----------------|
| 🌱 **Bioenergy** | 50 MW | 13/16 plants | 0.897 GW | 33.2% |
| ⚫ **Coal** | 490 MW | 1/1 plants | 0.5 GW | 44.4% |
| 🔥 **Gas** | 490 MW | 12/12 plants | 7.43 GW | 55% |
| 🌋 **Geothermal** | 60 MW | 0/1 plants | 0.005 GW | 100% |
| ☀️ **Solar** | 200 MW | 0/10 plants | 0.853 GW | 100% |
| 🌊 **Windoff** | 200 MW | 46/52 plants | 39.1 GW | 100% |
| 💨 **Windon** | 200 MW | 9/27 plants | 4.75 GW | 100% |
| 🔋 **Pumped Storage** | 60 MW | 2/2 plants | 2.28 GW | 100% |


Announced and pre-construction projects are offered as options to the model for endogenous investment.
This is particularly useful for hydro and pumped storage where country-wise potential is not readily
available. Grid locations of all these units are preserved.

### CCS Retrofit Potential

| Fuel | Retrofit Host Capacity | Retrofit Potential |
|------|------------------------|-------------------|
| ⚫ **Coal** | 56 GW | 41.5 GW after capacity penalty |
| 🔥 **Gas**  | 89 GW  | 75 GW after capacity penalty |

---

## Data Sources & Coverage

### Base-Year Power Plant Specifications

- **Global Energy Monitor (GEM)** — Open-access database of individual power plants worldwide,
  including location, capacity, fuel type, commissioning year, and technical specifications.
- **International Renewable Energy Agency (IRENA)** — Global renewable energy capacity and generation
  statistics (2000–2022), disaggregated by country and technology.
- **EMBER Climate** — Global dataset tracking electricity generation, installed capacity, and emissions
  intensity (2000–2022).

### Enhanced Renewable Energy Characterization

- **GEM–REZoning–Atlite Integration** — Renewable energy units enriched with capacity factors from
  Atlite weather data and precise grid-cell locations from the REZoning database.
- Individual renewable plants receive location-specific capacity factors derived from 2013 hourly
  weather patterns.
- Plants mapped to 50×50 km REZoning grid cells for consistent spatial modelling.

### Data Processing Notes

| Metric | Value |
|--------|-------|
| **Individual Plant Coverage** | 94% of total capacity from plant-level GEM data |
| **Total Capacity Tracked** | 400 GW from all sources |
| **Plants Above Threshold** | 656 individual plants tracked |
| **Total Plants Processed** | 1331 plants in database |
| **Missing Capacity Added** | - **IRENA data**:
  - **hydro**: 11.23 GW
  - **bioenergy**: 1.12 GW
  - **solar**: 54.33 GW
  - **windon**: 0.71 GW |

---

## Model Files

- **Source Data:** `source_data/VerveStacks_JPN.xlsx` — full dataset in a model-agnostic format
- **VEDA Model Files:** Complete model ready for Veda-TIMES execution
- **Scenario Files:** AR6 climate scenarios and policy assumptions

---

## Quality Assurance

- Cross-validation between IRENA, EMBER, and UNSD statistics
- Capacity-generation consistency checks
- Technology classification verification
- Historical data reconciliation for base year (2022)
- Renewable resource potential validated against REZoning database
- Temporal analysis verified through statistical scenario methods

*For questions about specific data sources or methodology, refer to the
[VerveStacks Methods documentation](https://vervestacks.readthedocs.io/en/latest/).*

---
*Generated by VerveStacks Energy Model Processor*
