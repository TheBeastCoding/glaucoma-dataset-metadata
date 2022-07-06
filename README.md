# multichannel-glaucoma-benchmark-dataset
Public multi-channel benchmark dataset for Glaucoma classification.

## Objective
The objective of this glaucoma benchmark dataset is to compile all available public glaucoma datasets into a single large dataset. This dataset will standardize image metadata and multi-modal image/segmentation data into machine-learning-ready data. Additionally, the benchmark dataset will provide dataset-level metadata related to the image collection study for metadata analysis. All dataset instances have the following linking constraint: the optic nerve head cropped fundus image. 

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
- DRISHTI-GS1-train
- DRISHTI-GS1-test

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

## Special Dataset Collection Method Notes
- BIOMISA: This dataset has 4 experts give each image a glaucoma classification label. Images are included in this dataset only if the majority (3 or 4 experts) agree on a label. The rest are discarded.

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
- Types: Majority Consensus of the Glaucoma classification; 0 = healthy, 1 = glaucoma suspect; 2 = glaucoma
- Database: Name of original database that instance was pulled from
- Original Name: The original name or derived name using the terminology of the original database
- ONH: File path of the Optic Nerve Head image (if any)
- Fundus: File path of the fundus image (if any)
- fundus_od_seg: File path of the fundus Optic Disc segmentation map or soft map if multiple experts annotated (if any)
- fundus_oc_seg: File path of the fundus Optic Cup segmentation map or soft map if multiple experts annotated (if any)
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
- foveaX: X Coordinate of the Fovea in the Fundus Image
- foveaY: Y Coordinate of the Fovea in the Fundus Image
- papCenterX_expert1/2: ?
- papCenterX_expert1/2: ?
- vesOriginX_expert1/2: X Coordinate of the Optic Nerve Head Origin in the Fundus Image Given by Expert 1 or 2
- vesOriginY_expert1/2: Y Coordinate of the Optic Nerve Head Origin in the Fundus Image Given by Expert 1 or 2
- diskDiameter_expert1/2: Diameter of the Optic Disk from the Fundus image Given by Expert 1 or 2
- notchI_present: Is notching present in the Inferior Fundus quandrant?
- notchS_present: Is notching present in the Superior Fundus quandrant?
- notchN_present: Is notching present in the Nasal Fundus quandrant?
- notchT_present: Is notching present in the Temporal Fundus quandrant?
- expert1_grade: Glaucoma classification from expert 1; 0 = healthy, 1 = glaucoma suspect; 2 = glaucoma
- expert2_grade: Glaucoma classification from expert 2; 0 = healthy, 1 = glaucoma suspect; 2 = glaucoma
- expert3_grade: Glaucoma classification from expert 3; 0 = healthy, 1 = glaucoma suspect; 2 = glaucoma
- expert4_grade: Glaucoma classification from expert 4; 0 = healthy, 1 = glaucoma suspect; 2 = glaucoma
- expert5_grade: Glaucoma classification from expert 5; 0 = healthy, 1 = glaucoma suspect; 2 = glaucoma
- cdr_avg: Average CDR estimation from all experts
- cdr_expert1: CDR estimation from expert 1
- cdr_expert2: CDR estimation from expert 2
- cdr_expert3: CDR estimation from expert 3
- cdr_expert4: CDR estimation from expert 4

## Original Public Dataset Sources and Citations

## Cite this dataset
