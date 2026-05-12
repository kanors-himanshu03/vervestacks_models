# IDN — VerveStacks ESOM Model

!!! info "Model Run"
    **Generated:** 2026-05-12 17:30:21  |  **ISO Code:** `IDN`

---

## Model Calibration 2022

| **Total Capacity** | **Total Generation** | **CO2 Emissions** | **Calibration to EMBER** |
|--------------|---------------|------------|--------------------------|
| 81 GW | 334 TWh | 225 Mt | 100% |

> **Note:** 2022 fossil and bio capacity is calibrated to EMBER and renewable capacities to IRENA.
> UNSD has incomplete data for fuel consumption, so calibration is demonstrated against total CO₂ emissions
> reported by EMBER — confirming that efficiency assumptions are sound.

---

## Power Generation Assets

### Existing Capacity

| **Fuel Type** | **Threshold** | **Plants Above Threshold** | **Active Capacity** | **Mothballed Capacity** | **Wtd Avg Efficiency** |
|---------------|---------------|----------------------------|--------------------|--------------------------|-----------------|
| 🌱 **Bioenergy** | 50 MW | 5/6 plants | 3.98 GW | — | 31% |
| ⚫ **Coal** | 140 MW | 153/211 plants | 63 GW | — | 36.2% |
| 🔥 **Gas** | 140 MW | 57/85 plants | 26 GW | 0.145 GW | 47.8% |
| 🌋 **Geothermal** | 10 MW | 55/57 plants | 3.19 GW | — | 100% |
| 💧 **Hydro Power** | 10 MW | 53/53 plants | 9.26 GW | — | 89% |
| 🛢️ **Oil** | 140 MW | 3/7 plants | 0.865 GW | — | 31.8% |
| ☀️ **Solar** | 200 MW | 0/22 plants | 0.678 GW | — | 96% |
| 💨 **Windon** | 200 MW | 0/3 plants | 0.157 GW | — | 100% |
| 🔋 **Pumped Storage** | 10 MW | 1/1 plants | 1.04 GW | — | 100% |


### Future Projects (offered for endogenous selection)

| **Fuel Type** | **Threshold** | **Plants Above Threshold** | **Total Capacity** | **Wtd Avg Efficiency** |
|---------------|---------------|----------------------------|--------------------|-----------------|
| ⚫ **Coal** | 140 MW | 4/4 plants | 4.86 GW | 34.5% |
| 🔥 **Gas** | 140 MW | 16/20 plants | 9.17 GW | 49.2% |
| 🌋 **Geothermal** | 10 MW | 39/39 plants | 2.78 GW | 100% |
| 💧 **Hydro Power** | 10 MW | 33/33 plants | 14.6 GW | 100% |
| ⚛️ **Nuclear** | — | 7/7 plants | 3.5 GW | 100% |
| ☀️ **Solar** | 200 MW | 18/26 plants | 16.5 GW | 100% |
| 💨 **Windon** | 200 MW | 3/12 plants | 1.52 GW | 100% |
| 🔋 **Pumped Storage** | 10 MW | 3/3 plants | 2.4 GW | 100% |


Announced and pre-construction projects are offered as options to the model for endogenous investment.
This is particularly useful for hydro and pumped storage where country-wise potential is not readily
available. Grid locations of all these units are preserved.

### CCS Retrofit Potential

| Fuel | Retrofit Host Capacity | Retrofit Potential |
|------|------------------------|-------------------|
| ⚫ **Coal** | 63 GW | 42.8 GW after capacity penalty |
| 🔥 **Gas**  | 26.2 GW  | 22.1 GW after capacity penalty |

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
| **Individual Plant Coverage** | 95% of total capacity from plant-level GEM data |
| **Total Capacity Tracked** | 164 GW from all sources |
| **Plants Above Threshold** | 399 individual plants tracked |
| **Total Plants Processed** | 589 plants in database |
| **Missing Capacity Added** | - **IRENA data**:
  - **hydro**: 1.49 GW
  - **geothermal**: 0.05 GW |

---

## Model Files

- **Source Data:** `source_data/VerveStacks_IDN.xlsx` — full dataset in a model-agnostic format
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

*For questions about specific data sources or methodology, refer to
[VerveStacks Methodology Documentation](https://github.com/VerveStacks/vervestacks/blob/main/docs/METHODOLOGY_DOCUMENTATION.md).*

---
*Generated by VerveStacks Energy Model Processor*
