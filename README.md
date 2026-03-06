

## Information on Data Collection

Samples were collected using **sediment cores** from a shallow-water benthic community in **Terrebonne Bay, Louisiana**.

Environmental data (water temperature, salinity, dissolved oxygen, chlorophyll) was gathered from the **Environmental Monitoring Program at the Louisiana Marine Consortium (LUMCON)** for the years **2018–2023**. Data were obtained from the **Terrebonne Bay** and **LUMCON monitoring stations**.

Only **macrofaunal invertebrates** were analyzed for this dataset.

---

# Data Files in Package

## `TB2B_CoreData.csv`
Relevant sampling, environmental, and sediment core data for site **TB2B**.

**Variables**

- **Sample ID** – Unique identifier for each sediment core from site TB2B with the notation  
  `[Station-Sampling Code-Core Number]`  
  Example: `TB2B-18.6-17`

- **Station** – Sampling site of each collected sediment core  
  Example: `TB2B`

- **Collection Date** – Date each sediment core was collected  
  Format: `Day/Month/Year`  
  Example: `6/14/18`

- **Sampling Code** – Unique code for each sampling event  
  Format: `[Year.Month]`  
  Example: `18.6`

- **Sample Event** – Unique identifier for each sampling event  
  Format: `[Year.Month.Number]`  
  Example: `18.06.1`

- **Grab** – Ponar grab number used during sampling  
  Example: `2`

- **Core** – Core number for each collected sediment core  
  Example: `17`

- **Year** – Year of sediment core collection  
  Example: `2018`

- **Month** – Month of sediment core collection  
  Example: `June`

- **Season** – Meteorological season of collection (Northern Hemisphere)  
  - Winter (December–February)  
  - Spring (March–May)  
  - Summer (June–August)  
  - Fall (September–November)

- **Months_Since_Hurricane** – Number of months since a hurricane event  
  Pre-hurricane samples labeled as `"Pre"`  
  Example: `1`

---

### Location Information

- **Latitude_DD** – Latitude in decimal degrees  
  Example: `29.178333°`

- **Longitude_DD** – Longitude in decimal degrees  
  Example: `-90.540500°`

- **Latitude_DMS** – Latitude in degrees/minutes/seconds  
  Example: `29° 10.700' N`

- **Longitude_DMS** – Longitude in degrees/minutes/seconds  
  Example: `90° 32.430' W`

- **Depth_m** – Water depth at sampling location (meters)  
  Example: `3.1`

---

### Environmental Variables (30 days prior to collection)

**Temperature**
- `max_temp_C`, `min_temp_C`, `mean_temp_C`
- `max_temp_F`, `min_temp_F`, `mean_temp_F`

**Salinity**
- `max_salinity_ppt`
- `min_salinity_ppt`
- `mean_salinity_ppt`

**Dissolved Oxygen**
- `max_DO_mg/L`
- `min_DO_mg/L`
- `mean_DO_mg/L`

**Chlorophyll**
- `max_chlorophyll_ug/L`
- `min_chlorophyll_ug/L`
- `mean_chlorophyll_ug/L`

---

### Core Quality Metrics

- **Water Loss** – Water loss during collection  
  - `None`
  - `Water Drain`
  - `Spill`  
  *(Contributes 0–1 point to core quality)*

- **Mud Disturbance** – Disturbance during collection  
  - `None`
  - `Slant`
  - `Split`
  - `Wonky`  
  *(Contributes 0–1 point to core quality)*

- **Mud Amount** – Amount of sediment collected (target = 5 cm)  
  - `Perfect` = 5 cm  
  - `Scant` = 4.9 cm  
  - `Scantish` = 4.8 cm  
  *(Contributes 0–5 points to core quality)*

- **Mud Loss** – Sediment lost during processing  
  Example: `0 cm`  
  *(1 spoonful ≈ 0.5 cm; contributes 0–2 points)*

- **Preservation** – Preservation state during processing  
  - `Preserved`
  - `Low EtOH`
  - `Dried Out`
  - `Desiccated`  
  *(Contributes 0–1 point to core quality)*

- **Core Quality** – Overall quality score  
  - `10` = perfect  
  - `9` = high quality  
  - `8` = moderate quality  
  - `7` = low quality  
  - `≤6` = core discarded

- **Status** – Processing status  
  - `Completed`
  - `Not Started`
  - `In Progress`
  - `Missing`
  - `Discarded`

---

## `TB2B_Taxa.csv`
Taxonomic and ecological information for each species.

**Variables**

- **Species ID** – Identifier matching the species matrix
- **Group** – General grouping for naming
- **Phylum, Class, Order, Family, Genus, Species** – Taxonomic classification
- **Synonymies** – Alternative names or nicknames
- **Body Size** – Mean biovolume of species (mm³)

Biovolume calculation:
1. Surface area measured using **ImageJ**
2. Multiplied by width/height/length

- **Notes** – Additional species information

---

## `TB2B_CoreByTaxa_With_Juv.csv`
Sample × species abundance matrix including juvenile individuals.

**Structure**

- **First column** – Sample identifiers
- **First row** – Species identifiers
- **Cell values** – Abundance of each species in each sample

**Example**

Column `C2` contains the abundance of species **Biv-2** in sample `TB2B-18.6-17`.

---
