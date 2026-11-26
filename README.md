# Tae-Hyung Kim

[![ORCID](https://img.shields.io/badge/ORCID-0009--0003--5047--7501-a6ce39?logo=orcid&logoColor=white)](https://orcid.org/0009-0003-5047-7501)
[![HelioStack PyPI](https://img.shields.io/pypi/v/heliostack.svg?label=heliostack)](https://pypi.org/project/heliostack/)
[![HelioStack Demo](https://img.shields.io/badge/Demo-HelioStack_Workbench-0f766e)](https://ttthkim-hue.github.io/heliostack/)
[![OpenFAIR-Mat Demo](https://img.shields.io/badge/Demo-OpenFAIR--Mat-2563eb)](https://ttthkim-hue.github.io/openfair-mat/)

**Computational Thermo-Fluids, Solar PV & Open-Science Systems Engineer** · Republic of Korea · `ttthkim@gmail.com`

Building deterministic, cryptographically auditable (`RO-Crate 1.1` + `SHA-256`), zero-runtime-AI open engineering tools that replace closed commercial silos—helping **individuals, citizen energy communities, small installers, and graduate researchers** design and verify solar PV, battery storage, and thermo-fluid systems on open standards.

---

## Featured Open-Source Stack

### 1. [`heliostack`](https://github.com/ttthkim-hue/heliostack) — Open Solar PV, OpenFOAM Thermal & ESS Workbench (`v0.3.2` · `AGPL-3.0-or-later`)
- **Install & Live Tools:** `pip install heliostack` ([PyPI](https://pypi.org/project/heliostack/)) · [Live Browser Workbench](https://ttthkim-hue.github.io/heliostack/) · [Zenodo DOI](https://doi.org/10.5281/zenodo.24491741) · [v1.0 Roadmap](https://github.com/ttthkim-hue/heliostack/blob/main/docs/ROADMAP.md)
- **What It Solves:** Frees PV + `LiFePO4` ESS simulation from Windows-only proprietary binaries (`PVsyst`, `PV*SOL`, `HOMER Pro`) and closed SaaS (`HelioScope`), empowering individuals, citizen energy cooperatives, local installers, and academic labs with local data sovereignty and `0%` runtime generative AI.
- **Verified Engineering & Telemetry:**
  - Clean-room `.PAN`/`.OND` single-diode & MPPT invariant checks, vectorized 3D ray-box obstacle shading, and **Copernicus GLO-30 DEM** 36-azimuth Alpine horizon ray-casting (`MAE 1.25–1.57°` across Innsbruck, Bolzano, Zermatt vs. EU PVGIS `printhorizon`).
  - **OpenFOAM 14** (`foamRun -solver fluid`, `5,910` cells, steady `kOmegaSST`) `28°`-tilted PV thermal sweep demonstrating `-3.59 °C` to `-5.77 °C` Floating-PV cooling vs. `0.08` dark-water albedo net bifacial tradeoff (`+0.38%` Seville vs. `-0.68%` Amsterdam).
  - **1-Year EU Field Validation** (University of Cyprus PHAETHON CoE, `8,784` hrs, `CC-BY-4.0`): `Tmod RMSE 2.18 °C` (`open_rack R² = 0.9705`), zero-tuned OpenFOAM `RMSE 4.19 °C` (`R² = 0.8906`), full-year DC `R² = 0.9887`.
  - **US Utility Telemetry** (US DOE / NREL PVDAQ `#2107`, `892.8 kWp`, `3,255` hrs): `R² = 0.9101`, `MBE = +3.81%`, `nRMSE = 6.79%`; plus canonical `pvlib ModelChain` parity (`-0.67%` Amsterdam, `+0.31%` Seville), `< 0.8 s` 8,760-hr sparse HiGHS `LiFePO4` curtailment LP, and `RO-Crate 1.1` provenance.

### 2. [`taichi_lbm_ref_gyroid`](https://github.com/ttthkim-hue/taichi_lbm_ref_gyroid) — GPU D3Q19 MRT-LBM CFD & Bayesian Optimization
- GPU-accelerated (`Taichi`) **D3Q19 Multiple-Relaxation-Time Lattice Boltzmann Method (MRT-LBM)** solver for Gyroid Triply Periodic Minimal Surface (TPMS) porous structures.
- Coupled with **Bayesian Optimization** (`100` evaluations, `50`-point Pareto front) over unit-cell size and level-set threshold, including GHSV sensitivity, Forchheimer nonlinear regression, `< 0.1%` repeatability CV, and OpenSCAD/STL/STEP geometry exchange.

### 3. [`openfair-mat`](https://github.com/ttthkim-hue/openfair-mat) — Pre-Flight Scientific Data & `RO-Crate 1.1` Validator (`v0.1.0` · `MIT`)
- Pure Python standard-library (`>= 3.10`, zero external AI/GPU dependencies) CLI (`openfair-check`) and [Live Browser Demo](https://ttthkim-hue.github.io/openfair-mat/) validating physical invariants and schemas across CIF, VASP `POSCAR`/`CONTCAR`, and tabular CSV/JSON datasets.
- Auto-generates `RO-Crate 1.1` (`ro-crate-metadata.json`) and `SHA-256` (`repro-manifest.json`) readiness bundles for **Zenodo (CERN)**, **NOMAD (FAIRmat)**, and **Materials Project**.

---

## Academic Background & Scientific Competitions

- **M.S. in Materials Engineering**, Pusan National University (`2025`) — Master's Thesis: *"CO₂ Curable Cementitious Materials for Binder Jet 3D Printing"*; Principal Investigator, *2023 PNU Convergence Creative Project*.
- **B.S. in Materials Engineering**, University of Ulsan (`2020`).
- **MVA2027 SMOTP4SB Track 2** (Small-Object Trajectory Prediction, [CodaBench #18323](https://www.codabench.org/competitions/18323/)): Reached **Public Test #1** peak; verified Top-3 standing (`SO-HOTA-TP = 0.1835` as of `2026-11-20`).

---

## Peer-Reviewed Publications

**14 peer-reviewed journal articles indexed on [ORCID `0009-0003-5047-7501`](https://orcid.org/0009-0003-5047-7501)** (**7 sole first-author**, **1 co-first author**, **6 co-author**), plus **1 additional 2022 Crossref/OpenAlex-verified co-authored article** (**15 total verified works**).

### First-Author & Co-First-Author Articles (8)

| Year | Role | Title | Journal | DOI |
| :---: | :---: | :--- | :--- | :--- |
| 2026 | **First Author** | Self-powered triboelectric electrospun air filters as functional fibrous materials: Experiment-supported modeling of dielectrophoretic capture and scale-up | *Materials Today Communications*, 56, 115941 | [`10.1016/j.mtcomm.2026.115941`](https://doi.org/10.1016/j.mtcomm.2026.115941) |
| 2026 | **Co-First Author** | Characteristics of calcium silicate cement: Effects of CO2 curing and CaCO3 micro-filler addition | *Journal of the Ceramic Society of Japan*, 134(6), 398–404 | [`10.2109/jcersj2.25126`](https://doi.org/10.2109/jcersj2.25126) |
| 2026 | **First Author** | Burnability of High-Performance Cement Clinker Using KR Slag and Reduction Slag | *Resources Recycling*, 35(1), 43–55 | [`10.7844/kirr.2026.35.1.43`](https://doi.org/10.7844/kirr.2026.35.1.43) |
| 2025 | **First Author** | A Self-Powered Cationic Microfiber-Based Triboelectric Air Filter for High-Speed Particulate Matter Removal and Smart Monitoring | *Journal of Powder Materials*, 32(6), 481–491 | [`10.4150/jpm.2025.00465`](https://doi.org/10.4150/jpm.2025.00465) |
| 2025 | **First Author** | Production of Hydrated Lime for Flue Gas De-sulfurization via Dry Slaking Process | *Resources Recycling*, 34(1), 33–43 | [`10.7844/kirr.2025.34.1.33`](https://doi.org/10.7844/kirr.2025.34.1.33) |
| 2025 | **First Author** | Rheology control of CO2 curable ceramic powder for binder jetting | *Advanced Powder Technology*, 36(1), 104729 | [`10.1016/j.apt.2024.104729`](https://doi.org/10.1016/j.apt.2024.104729) |
| 2024 | **First Author** | Production of High-Strength Cement Clinker Using Slag-Based Industrial By-Products | *Resources Recycling*, 33(6), 64–74 | [`10.7844/kirr.2024.33.6.64`](https://doi.org/10.7844/kirr.2024.33.6.64) |
| 2024 | **First Author** | Influence of CaCO3 on Density and Compressive Strength of Calcium Aluminate Cement-Based Cementitious Materials in Binder Jetting | *Materials*, 17(14), 3463 | [`10.3390/ma17143463`](https://doi.org/10.3390/ma17143463) |

### Co-Authored Peer-Reviewed Articles (7)

| Year | Role | Title | Journal | DOI |
| :---: | :---: | :--- | :--- | :--- |
| 2026 | Co-author | Facile Etching Process for the Porous Structure of Hexagonal Boron Nitride as a Catalyst Support Using Metal Oxides Under Low-Temperature Conditions | *Catalysts*, 16(9), 837 | [`10.3390/catal16090837`](https://doi.org/10.3390/catal16090837) |
| 2026 | Co-author | Current Status and Applications of Organic Rankine Cycles in the Global Cement Industry | *Resources Recycling*, 35(2), 30–41 | [`10.7844/kirr.2026.35.2.30`](https://doi.org/10.7844/kirr.2026.35.2.30) |
| 2026 | Co-author | Boosting NH3-Selective Catalytic Reduction of NOx by Cooperation of Nb and Boron Nitride to V-Based Catalyst over a Wide Temperature Window | *Applied Nano*, 7(1), 9 | [`10.3390/applnano7010009`](https://doi.org/10.3390/applnano7010009) |
| 2025 | Co-author | Analysis of Alternative Fuels for Carbon Reduction in the Cement Industry | *Resources Recycling*, 34(5), 18–31 | [`10.7844/kirr.2025.34.5.18`](https://doi.org/10.7844/kirr.2025.34.5.18) |
| 2025 | Co-author | Development of a Continuous Process for High Surface Area Slaked Lime Depending on Additive Mixing Methods and Drying Temperature | *Resources Recycling*, 34(1), 68–74 | [`10.7844/kirr.2025.34.1.68`](https://doi.org/10.7844/kirr.2025.34.1.68) |
| 2024 | Co-author | Liquid Nitrogen Exfoliation and Nanodispersion of WS2 for Thermocatalysts | *ACS Applied Materials & Interfaces*, ASAP (`acsami.4c11888`) | [`10.1021/acsami.4c11888`](https://doi.org/10.1021/acsami.4c11888) |
| 2022 | Co-author | Penetrated surface characteristics of cement - mixed sand in powder bed 3D printing | *Journal of Asian Ceramic Societies*, 10(2), 306–313 *(Crossref/OpenAlex verified)* | [`10.1080/21870764.2021.2024734`](https://doi.org/10.1080/21870764.2021.2024734) |
