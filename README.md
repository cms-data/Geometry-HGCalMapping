# Geometry-HGCalMapping

Data files for Geometry/HGCalMapping

The contents are stored under three directories:
- CellMaps
  - Si cell mapping: contains the correspondence of geometry location to readout sequence for each different hexaboard type
  - SiPM-on-tile cell mapping: similar as the previous, for the tileboards
- ModuleMaps
  - Module mapping: contains the correspondence between the geometry location of each module and it's indexing in the readout sequence
- DQM
  - Templates and metadata for the HGCAL DQM plugins (DQM/HGCAL)

Cell maps are expected to be fixed describing each board type.
Module maps may vary. The current versions available are:

| File | Description |
|---|---|
| `modulelocator_test.txt` | dummy, for testing purposes |
| `modulelocator_CEminus_V15p5.txt` | generated from modmap v15.5 |

The DQM files are:

| File | Description |
|---|---|
| `geometry_<type>_TC_wafer.root` | trigger cells in a module |
| `geometry_<type>_wafer.root`, `geometry_<type>_tileboard.root` | DAQ channels in a module |
| `geometry_v16p6.root` | all HGCAL modules |
| `dqm_quality_threshold.json` | metadata for the DQM plugins |

