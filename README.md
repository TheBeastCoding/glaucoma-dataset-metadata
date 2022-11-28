# Public Glaucoma Dataset Catalog and Standardized Glaucoma Dataset
All public glaucoma datasets are documented and a novel multi-channel benchmark dataset is presented, which standardizes all public glaucoma datasets into a single, large dataset.

## Cite this dataset
- *INSERT CITATION HERE*

## Public Glaucoma Image Datasets
| Dataset   | Access Link | Accessibility | Glaucoma Labels? | Included in our dataset? |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| ACRIMA  | https://figshare.com/s/c2d31f850af14c5b5232  | open | Y | Y |
| AGE  | https://age.grand-challenge.org/Download/  | registration | Y | N |
| BEH (Bangladesh Eye Hospital) | https://github.com/mirtanvirislam/Deep-Learning-Based-Glaucoma-Detection-with-Cropped-Optic-Cup-and-Disc-and-Blood-Vessel-Segmentation/tree/master/Dataset | open | Y | Y |
| BIOMISA | https://data.mendeley.com/datasets/2rnnz5nz74/2  | open | Y | Y |
| CRFO-v4 | https://data.mendeley.com/datasets/trghs22fpg/4 | open | Y | Y |
| DR-HAGIS | https://personalpages.manchester.ac.uk/staff/niall.p.mcloughlin/ | open | Y | Y |
| DRIONS-DB  | https://www.researchgate.net/publication/326460478_Glaucoma_dataset_-_DRIONS-DB  | open | N | N |
| DRISHTI-GS1  | https://cvit.iiit.ac.in/projects/mip/drishti-gs/mip-dataset2/Home.php  | open | Y | Y |
| EyePACS-AIROGS | https://airogs.grand-challenge.org/data-and-challenge/ | open | Y | Y |
| G1020 | https://www.kaggle.com/datasets/arnavjain1/glaucoma-datasets | open | Y | Y |
| GAMMA | https://gamma.grand-challenge.org/ | registration | Y | N |
| GOALS | https://goals.grand-challenge.org/ | registration | Y | N |
| HRF  | https://www5.cs.fau.de/research/data/fundus-images/  | open | Y | Y |
| JSIEC-1000 | https://www.kaggle.com/datasets/linchundan/fundusimage1000 | registration | Y | Y |
| KEH (Kim's Eye Hospital) | https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/1YRRAC | open | Y | Y |
| INSPIRE-AVR-test | https://medicine.uiowa.edu/eye/inspire-datasets | open | N | N |
| INSPIRE-STEREO | https://medicine.uiowa.edu/eye/inspire-datasets | open | N | N |
| LAG | https://github.com/smilell/AG-CNN | request | Y | N |
| LES-AV | https://figshare.com/articles/dataset/LES-AV_dataset/11857698/1 | open | Y | Y |
| OCTV | https://zenodo.org/record/1481223#.Y20g3XbMIuV | open | Y | N |
| OIA-ODIR | https://www.kaggle.com/datasets/andrewmvd/ocular-disease-recognition-odir5k | registration | Y | Y |
| ONHSD | https://aldiri.info/Image%20Datasets/ONHSD.aspx | inaccessible | Y | N |
| ORIGA-light | https://www.kaggle.com/datasets/sshikamaru/glaucoma-detection | registration | Y | Y |
| PAPILA | https://doi.org/10.6084/m9.figshare.14798004.v1 | open | Y | Y |
| REFUGE1  | https://refuge.grand-challenge.org/REFUGE2Download/  | registration | Y | Y |
| REFUGE2  | https://refuge.grand-challenge.org/REFUGE2Download/  | registration | Y | Y |
| RIGA-BIN-RUSHED | https://deepblue.lib.umich.edu/data/concern/data_sets/3b591905z  | open | N | N |
| RIGA-MAGRABI | https://deepblue.lib.umich.edu/data/concern/data_sets/3b591905z  | open | N | N |
| RIGA-MESSIDOR | https://deepblue.lib.umich.edu/data/concern/data_sets/3b591905z  | open | N | N |
| RIM-ONE-r1 | http://medimrg.webs.ull.es/research/retinal-imaging/rim-one/  | open | Y | N |
| RIM-ONE-r2 | http://medimrg.webs.ull.es/research/retinal-imaging/rim-one/  | open | Y | N |
| RIM-ONE-r3 | http://medimrg.webs.ull.es/research/retinal-imaging/rim-one/  | open | Y | N |
| RIM-ONE-DL | http://medimrg.webs.ull.es/research/retinal-imaging/rim-one/  | open | Y | N |
| SIGF | https://github.com/XiaofeiWang2018/DeepGF | request | Y | N |
| sjchoi86-HRF | https://github.com/yiweichen04/retina_dataset | open | Y | Y |
| VEIRC | https://github.com/ProfMKD/Glaucoma-dataset | open | Y | N |

## Dataset Survey Objective
The objective of this glaucoma dataset survey is to document existing datasets and their corresponding metadata and attributes. Please see dataset-metadata.csv.

## Sampled Dataset Objective
The objective of the the sampeld dataseet is to take a selection of 2 glaucoma samples and 2 non-glaucoma samples from each dataset (if available) and document additional clinical features via expert analysis.

## Standardized Dataset Objective
The objective of this glaucoma benchmark dataset is to compile all available public glaucoma datasets into a single large dataset. This dataset will standardize image metadata and multi-modal image/segmentation data into machine-learning-ready data. Additionally, the benchmark dataset will provide dataset-level metadata related to the image collection study for metadata analysis. All dataset instances have the following linking constraint: the optic nerve head cropped fundus image. 

## Standardized Dataset Summary
- There are 14,467 unique dataset instances with their own unique channel information.
- 8,681 instaces are non-glaucoma
- 5,773 instances are glaucoma
- 133 instances are glaucoma suspect

## Image Standardization Examples
### Raw Fundus Standardization
Original Fundus (sjchoi86-HRF) |  Background Cropped and Resized to 512x512 with Aspect Resolution Preservation
--- | ---
![fundus](https://user-images.githubusercontent.com/65875562/204170005-2d4dd051-0032-40c8-ba0b-390b6080bb69.png) | ![fundus_cropped](https://user-images.githubusercontent.com/65875562/204170011-51b7d001-4d43-4f0d-835e-984d45116b18.png)

### Optic Cup/Disc Standardization
Standardized Fundus Image (Drishti-GS)
--- | ---
![fundus](https://user-images.githubusercontent.com/65875562/204174106-efcf4de1-3cc3-4bbc-ac46-8e9d05d46be6.png) | ![fundus_standardized](https://user-images.githubusercontent.com/65875562/204173700-c3ce6680-c317-4b6e-a5b0-c30ea7d25339.png)

## Standardized Dataset Data Access Link
https://www.kaggle.com/datasets/deathtrooper/multichannel-glaucoma-benchmark-dataset [The dataset will be published in late 2022]

## The following datasets were used in the creation of this benchmark dataset.
- ACRIMA
- OIA-ODIR-TRAIN
- OIA-ODIR-TEST-ONLINE
- OIA-ODIR-TEST-OFFLINE
- HRF (High Resolution Fundus)
- LES-AV
- sjchoi86-HRF
- BEH (Bangladesh Eye Hospital)
- REFUGE1-TRAIN (Retinal Fundus Glaucoma Challenge 1 Train)
- REFUGE1-VAL (Retinal Fundus Glaucoma Challenge 1 Validation)
- DR-HAGIS (Diabetic Retinopathy, Hypertension, Age-related macular degeneration and Glacuoma ImageS)
- CRFO-v4
- JSEIC-1000 (Joint Shantou International Eye Center)
- DRISHTI-GS1-train
- DRISHTI-GS1-test
- KEH (Kim's Eye Hospital)
- G1020
- EyePACS-AIROGS (Referable Glaucoma Images Only)
- PAPILA

## Benchmark Dataset File Structure
- Glaucoma Suspect (-1)
  - Glaucoma Suspect Instance 1
    - channel image data (fundus, oct, optic disc, ...)
  - ...
- Glaucoma (1)
  - Glaucoma Instance 1
    - channel image data (fundus, oct, optic disc, ...)
  - ...
- Non-Glaucoma (0)
  - Non-Glaucoma Instance 1
    - channel image data (fundus, oct, optic disc, ...)
  - ...
- metadata.csv
  - complete documentation of instance attributes (sex, age, eye, ...)

## Special Dataset Collection Method Notes
- BIOMISA: This dataset has 4 experts give each image a glaucoma classification label. Images are included in this dataset only if the majority (3 or 4 experts) agree on a label. The rest are discarded.
- Datasets that reported their own fundus FOV segmentation data are discarded. All FOV segmentations are calcualted by our own algorithm.

## Instance Image Data Channel Options (Note: for segmentation maps, white pixels represent area of interest)
- fundus.*; Raw Fundus Image
- fundus_cropped.png; Raw Fundus Image Cropped to Remove Additional Background
- fundus_standardized.png; Raw Fundus Image Cropped to Remove Additional Background and Resized to 512x512 with aspect resolution preservation via padding with black pixels
- oct.*; OCT Image: Optical Coherence Tomography B-Scan
- onh.*; ONH Image: Cropped fundus image showing the Optic Nerve Head and some periperhal area
- fundus_od.*; Fundus OD Map: Fundus Optic Disc Segmentation Map
- fundus_od_seg_cropped.png; Raw Fundus Optic Disc Segmentation Map Cropped to Remove Additional Background
- fundus_od_seg_standardized.png; Raw Fundus Optic Disc Segmentation Map Cropped to Remove Additional Background and Resized to 512x512 with aspect resolution preservation via padding with black pixels
- fundus_oc.*; Fundus OC Map: Fundus Optic Cup Segmentation Map
- fundus_oc_seg_cropped.png; Raw Fundus Optic Cup Segmentation Map Cropped to Remove Additional Background
- fundus_oc_seg_standardized.png; Raw Fundus Optic Cup Segmentation Map Cropped to Remove Additional Background and Resized to 512x512 with aspect resolution preservation via padding with black pixels
- oct_od.*; OCT OD Map: OCT Optic Disc Segmentation Map
- oct_oc.*; OCT OC Map: OCT Optic Cup Segmentation Map
- fov.*; FOV Map: Raw Fundus Field of View Segmentation Map
- fundus_fov_seg_cropped.png; Raw Fundus Field of View Segmentation Map Cropped to Remove Additional Background
- fundus_fov_seg_standardized.png; Raw Fundus Field of View Segmentation Map Cropped to Remove Additional Background and Resized to 512x512 with aspect resolution preservation via padding with black pixels
- bv.*; BV Map: Raw Fundus Blood Vessel Segmentation Map
- bv_seg_cropped.png; Raw Fundus Blood Vessel Segmentation Map Cropped to Remove Additional Background
- bv_seg_standardized.png; Raw Fundus Blood Vessel Segmentation Map Cropped to Remove Additional Background and Resized to 512x512 with aspect resolution preservation via padding with black pixels
- artery.*; Artery Map: Artery Segmentation Map
- artery_seg_cropped.png; Raw Fundus Artery Segmentation Map Cropped to Remove Additional Background
- artery_seg_standardized.png; Raw Fundus Artery Segmentation Map Cropped to Remove Additional Background and Resized to 512x512 with aspect resolution preservation via padding with black pixels
- vein.*; Vein Map: Vein Segmentation Map
- vein_seg_cropped.png; Raw Fundus Vein Segmentation Map Cropped to Remove Additional Background
- vein_seg_standardized.png; Raw Fundus Vein Segmentation Map Cropped to Remove Additional Background and Resized to 512x512 with aspect resolution preservation via padding with black pixels

## Metadata CSV Attribute Listing and Explaination
- Names: Instance name; includes database name and instance number
- Types: Majority Consensus of the Glaucoma classification; 0 = Non-Glaucoma, -1 = glaucoma suspect; 1 = glaucoma
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
- expert1_grade: Glaucoma classification from expert 1; 0 = Non-Glaucoma, -1 = glaucoma suspect; 1 = glaucoma
- expert2_grade: Glaucoma classification from expert 2; 0 = Non-Glaucoma, -1 = glaucoma suspect; 1 = glaucoma
- expert3_grade: Glaucoma classification from expert 3; 0 = Non-Glaucoma, -1 = glaucoma suspect; 1 = glaucoma
- expert4_grade: Glaucoma classification from expert 4; 0 = Non-Glaucoma, -1 = glaucoma suspect; 1 = glaucoma
- expert5_grade: Glaucoma classification from expert 5; 0 = Non-Glaucoma, -1 = glaucoma suspect; 1 = glaucoma
- cdr_avg: Average CDR estimation from all experts
- cdr_expert1: CDR estimation from expert 1
- cdr_expert2: CDR estimation from expert 2
- cdr_expert3: CDR estimation from expert 3
- cdr_expert4: CDR estimation from expert 4
- glaucoma_type: Expert diagnoisis of glaucoma subtype (ex. early glaucoma, advanced glaucoma, open angle, closed angle, ...)
- oct:  File path of the Optical coherence tomography image (if any)
- patient_id: ID of the patient (if any) for test/retest cases or left and right eye for same patient
- refractive_dioptre_1: 
- refractive_dioptre_2:
- refractive_astigmatism: 
- phakic_or_pseudophakic:
- iop_perkins:
- iop_pneumatic:
- pachymetry:
- axial_length:
- visual_field_mean_defect:
- gender:
- fundus_height:
- fundus_width:
