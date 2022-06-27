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
- REFUGE1-VAL
- DR-HAGIS
- CRFO-v4
- JSEIC-1000

## Benchmark Dataset File Structure
- Glaucoma Suspect
  - Glaucoma Suspect Instance 1
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

## Instance Image Data Channel Options (Note: for segmentation maps, white pixels represent area of interest)
- Fundus Image
- OCT Image: Optical Coherence Tomography B-Scan
- ONH Image: Cropped fundus image showing the Optic Nerve Head and some periperhal area
- Fundus OD Map: Fundus Optic Disc Segmentation Map
- Fundus OC Map: Fundus Optic Cup Segmentation Map
- OCT OD Map: OCT Optic Disc Segmentation Map
- OCT OC Map: OCT Optic Cup Segmentation Map
- FOV Map: Fundus Field of View Segmentation Map
- BV Map: Blood Vessel Segmentation Map
- Artery Map: Artery Segmentation Map
- Vein Map: Vein Segmentation Map

## Metadata CSV Attribute Listing and Explaination
- Names: Instance name; includes database name and instance number
- Types: Glaucoma classification types; 0 = healthy, 1 = glaucoma suspect; 2 = glaucoma
- Database: Name of original database that instance was pulled from
- Original Name: The original name or derived name using the terminology of the original database
- ONH: File path of the Optic Nerve Head image (if any)
- Fundus: File path of the fundus image (if any)
- fundus_od_seg: File path of the fundus Optic Disc segmentation map (if any)
- fundus_oc_seg: File path of the fundus Optic Cup segmentation map (if any)
- fov_seg: File path of the fundus Field of View segmentation map (if any)
- bv_seg: File path of the fundus Blood Vessel segmentation map (if any)
- artery_seg: File path of the fundus Artery segmentation map (if any)
- vein_seg: File path of the fundus Vein segmentation map (if any)
- sex: Patient sex (if reported)
- age: Patient age (if reported)
- eye: Patient eye; OD = oculus dexter (right), OS = oculus sinister (left) (if reported)
- sbp: Patient systolic blood pressure (if reported)
- dbp: Patient dystolic blood pressure (if reported)
- hr: Patient heart rate (if reported)
- iop: Patient intra-ocular pressure (if reported)
- vcdr: Patient vertical cup to disk ratio (if reported)
- isColor: If reported fundus image is in color; 0 = grayscale, 1 = color (if reported)
- oct_od_seg: File path of the OCT Optic Disc segmentation map (if any)
- oct_oc_seg: File path of the OCT Optic Cup segmentation map (if any)
