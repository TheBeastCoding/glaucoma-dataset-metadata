# glaucoma-benchmark
Public multi-channel benchmark dataset for Glaucoma classification.

## The following datasets were used in the creation of this benchmark dataset.
- ACRIMA
- OIA-ODIR-TRAIN
- OIA-ODIR-TEST-ONLINE
- OIA-ODIR-TEST-OFFLINE
- HRF
- LES-AV
- sjchoi86-HRF
- BEH
- REFUGE1-TRAIN
- DR-HAGIS
- CRFO-v4
- JSEIC-1000

## Benchmark Dataset File Structure
- Suspect
  - Suspect Instance 1
    - channel image data (fundus, oct, optic disc, ...)
  - ...
- Glaucoma
  - Glaucoma Instance 1
    - channel image data (fundus, oct, optic disc, ...)
  - ...
- Healthy
  - Healthy Instance 1
    - channel image data (fundus, oct, optic disc, ...)
  - ...
- metadata.csv
  - complete documentation of instance attributes (sex, age, eye, ...)
