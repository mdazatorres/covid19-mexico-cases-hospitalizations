# COVID-19 Data for Mexico States and Metropolitan Areas

This repository provides COVID-19 data for states and metropolitan areas in Mexico, including confirmed cases, deaths, and hospital occupancy. Data is organized by **state/locality codes (claves)** and stored in structured CSV files.

---

## Repository Contents

### 1. `Clave.csv`
Contains time series of COVID-19 cases and deaths.

- **Column 0** → Deaths  
- **Column 1** → Cases  

### 2. `Clave_DinHospitales.csv`
Contains hospital occupancy data.

- **camasOcupadasHG** → Occupied beds (general medicine)  
- **camasOcupadasNumberUCIVentiladores** → Occupied general beds with ventilators  
- **camasOcupadasUCI** → Occupied beds in ICU  
- **camasOcupadasUCI_NumberofUCIVent** → Occupied ICU beds with ventilators  

### 3. `configuracion.csv`
Provides metadata and the mapping of **claves** to state or metropolitan names.

- Each state/metropolitan area has a unique clave.  
- Example:  
  - **Aguascalientes → clave: AS**  
  - Case and death file: `AS.csv`  
  - Hospitalization file: `AS_DinHospitales.csv`  

---

## Usage Example

To analyze data for **Aguascalientes**:

1. Load `AS.csv` for cases and deaths.  
2. Load `AS_DinHospitales.csv` for hospital occupancy.  
3. Use `configuracion.csv` to map `AS` to the state name and metadata.  

---

## Notes

- Data is available at the **state and metropolitan level**.  
- Ensure that the correct **clave** is used when linking files.  
- All files are provided in **CSV format**, suitable for analysis in Python, R, or other statistical tools.  

---

##  License and Citation

If you use this dataset in your research or publications, please cite the following articles:

1. Capistran M.A., Capella A., Christen J.A. (2021).  
   *Forecasting hospital demand in metropolitan areas during the current COVID-19 pandemic and estimates of lockdown-induced 2nd waves.*  
   **PLOS ONE**, 16(1): e0245669. https://doi.org/10.1371/journal.pone.0245669  

2. Daza-Torres M.L., Capistrán M.A., Capella A., Christen J.A. (2022).  
   *Bayesian sequential data assimilation for COVID-19 forecasting.*  
   **Epidemics**, 39: 100564. https://doi.org/10.1016/j.epidem.2022.100564  




