# PCEB Catalog

Associated data and code from the Post-Common Envelope Binary (PCEB) catalog.

## Overview

This repository contains the PCEB catalog from **Shariat & El-Badry (2026)**. The catalog presents a comprehensive analysis of white dwarf-main sequence (WDMS) binary systems, combining stellar parameters derived from spectroscopy and photometry with astrometric data from Gaia.

**Paper**: *[Link to be added upon publication]*

## Data

### wdms_pcebs.csv

The main catalog file `wdms_pcebs.csv` contains the full set of parameters for white dwarf-main sequence binary systems, including stellar properties and Gaia astrometric measurements.

#### Column Descriptions

| Column | Description |
|--------|-------------|
| `source_id` | Gaia DR3 source identifier |
| **Main Sequence Parameters** | |
| `Teff_ms_med` | Main sequence star effective temperature (K) - median value |
| `Teff_ms_errp` | Main sequence star effective temperature - upper error (K) |
| `Teff_ms_errm` | Main sequence star effective temperature - lower error (K) |
| `R_ms_med` | Main sequence star radius (R☉) - median value |
| `R_ms_errp` | Main sequence star radius - upper error (R☉) |
| `R_ms_errm` | Main sequence star radius - lower error (R☉) |
| `M_ms_med` | Main sequence star mass (M☉) - median value |
| `M_ms_errp` | Main sequence star mass - upper error (M☉) |
| `M_ms_errm` | Main sequence star mass - lower error (M☉) |
| `logg_ms_med` | Main sequence star surface gravity (log g) - median value |
| `logg_ms_errp` | Main sequence star surface gravity - upper error |
| `logg_ms_errm` | Main sequence star surface gravity - lower error |
| **White Dwarf Parameters** | |
| `Teff_wd_med` | White dwarf effective temperature (K) - median value |
| `Teff_wd_errp` | White dwarf effective temperature - upper error (K) |
| `Teff_wd_errm` | White dwarf effective temperature - lower error (K) |
| `M_wd_med` | White dwarf mass (M☉) - median value |
| `M_wd_errp` | White dwarf mass - upper error (M☉) |
| `M_wd_errm` | White dwarf mass - lower error (M☉) |
| `logg_wd_med` | White dwarf surface gravity (log g) - median value |
| `logg_wd_errp` | White dwarf surface gravity - upper error |
| `logg_wd_errm` | White dwarf surface gravity - lower error |
| **Gaia Parameters** | |
| `ra` | Right ascension (degrees) |
| `dec` | Declination (degrees) |
| `parallax` | Parallax (mas) |
| `parallax_error` | Parallax uncertainty (mas) |
| `pmra` | Proper motion in right ascension (mas/yr) |
| `pmra_error` | Proper motion in right ascension uncertainty (mas/yr) |
| `pmdec` | Proper motion in declination (mas/yr) |
| `pmdec_error` | Proper motion in declination uncertainty (mas/yr) |
| `phot_g_mean_mag` | Gaia G-band mean magnitude |
| `phot_bp_mean_mag` | Gaia BP-band mean magnitude |
| `phot_rp_mean_mag` | Gaia RP-band mean magnitude |
| `ruwe` | Renormalized unit weight error (astrometric quality indicator) |
| **Binary System Parameters** | |
| `period_med` | Orbital period (days) - median value |
| `period_errp` | Orbital period - upper error (days) |
| `period_errm` | Orbital period - lower error (days) |
| `separation_med` | Binary separation (AU) - median value |
| `separation_errp` | Binary separation - upper error (AU) |
| `separation_errm` | Binary separation - lower error (AU) |

#### Error Convention

All uncertainties are reported as asymmetric errors:
- `_errp`: Upper (positive) error bar
- `_errm`: Lower (negative) error bar, typically reported as an absolute value

#### Notes

- All parameter values with `_med` suffix represent the median of the posterior distribution from the analysis
- Missing values are indicated by `NaN` or empty cells
- The Gaia parameters are from Gaia Data Release 3 (DR3)

## Citation

If you use this catalog in your research, please cite:

```
Shariat & El-Badry (2026), [Journal], [Volume], [Page]
[ADS link to be added]
```

## Contact

For questions or issues regarding the catalog, please open an issue on this repository or contact the authors.

## License

See [LICENSE](LICENSE) file for details.
