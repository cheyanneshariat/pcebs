# Post Common Envelope Binaries (PCEBs)  
**Shariat & El-Badry (2026)**

---

## Overview

This repository contains the catalog of eclipsing detached PCEBs from Gaia DR3 and ZTF within 200 pc from the Sun. The catalog construction is detailed in Shariat & El-Badry (2026); please cite that paper when using this catalog. 

The contents of the repo are:

1. **`WDMS_EBs.csv`** Table of the **entire sample**, where **each row corresponds to one binary** eclipsing WDMS PCEB.

---

## Data Columns

This table contains observed and derived parameters for detached white dwarf+main-sequence PCEBs. Unless otherwise noted, all uncertainties are quoted as the 16th and 84th percentiles.

---

### Identifiers and astrometry
- **source_id**  
  Gaia DR3 source identifier
- **parallax**  
  Gaia parallax (mas)
- **reference**  
  Literature source for the system parameters
- **ref_letter**  
  Short reference label used in figures and tables

---

### Main-sequence companion (MS) parameters
All MS stellar parameters are derived from SED fitting.

- **Teff_ms_med**  
  Effective temperature (K)
- **Teff_ms_errm**, **Teff_ms_errp**  
  Lower and upper uncertainties on MS effective temperature
- **R_ms_med**  
  Radius (R⊙)
- **R_ms_errm**, **R_ms_errp**  
  Lower and upper uncertainties on MS radius
- **M_ms_fromR_med**  
  Mass inferred from the radius using stellar models (M⊙)
- **M_ms_fromR_errm**, **M_ms_fromR_errp**  
  Lower and upper uncertainties on MS mass

---

### White dwarf (WD) parameters
WD parameters are inferred photometrically via SED fitting and WD mass–radius relations.

- **Teff_wd_med**  
  Effective temperature (K)
- **Teff_wd_errm**, **Teff_wd_errp**  
  Lower and upper uncertainties on WD effective temperature
- **R_wd_med**  
  Radius (R⊙)
- **R_wd_errm**, **R_wd_errp**  
  Lower and upper uncertainties on WD radius
- **M_wd_fromR_med**  
  WD mass inferred from the radius (M⊙)
- **M_wd_fromR_errm**, **M_wd_fromR_errp**  
  Lower and upper uncertainties on WD mass
- **tau_cool**  
  WD cooling age (Gyr)
- **tau_cool_low**, **tau_cool_high**  
  Lower and upper bounds on WD cooling age

---

### Orbital parameters
- **ztf_period_hr**  
  Observed orbital period from ZTF light curves (hours)
- **P_days**  
  Orbital period converted to days

---

### Extinction and auxiliary data flags
- **EBV_fixed**  
  Adopted reddening value E(B−V)
- **has_real_EBV**  
  Boolean flag indicating whether E(B−V) was directly constrained
- **has_galex**  
  Boolean flag indicating availability of GALEX UV photometry

---

### Future evolution and magnetic braking
These quantities describe the predicted orbital evolution under magnetic braking.

- **P_RL_days**, **P_roche_days**  
  Orbital period at which the MS star fills its Roche lobe (days)
- **t_to_roche_Gyr_Sat**  
  Time until Roche–lobe overflow assuming saturated magnetic braking (Gyr)
- **t_RVJ_Gyr**  
  Time until Roche–lobe overflow assuming classical RVJ magnetic braking (Gyr)
- **t_SAT_Gyr**  
  Time until Roche–lobe overflow assuming the saturated S00 prescription (Gyr)

---

## Notes
- All masses are in solar units (M⊙), radii in solar units (R⊙), periods in days or hours as specified.
- Timescales are given in gigayears (Gyr).
- WD and MS parameters are derived independently via SED fitting.

---

## Contact

For questions regarding the data or analysis, please contact:  
**cshariat@caltech.edu**
