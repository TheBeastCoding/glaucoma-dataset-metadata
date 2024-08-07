## New Updates
* 08/03/24 : A new abstract is available to the public, introducing a novel approach to glaucoma detection: Assessment of Retinal Vasculature for Glaucoma Detection: A Comparative Analysis of Human Expertise and Deep Learning Algorithms.
* 05/15/24 : The EyePACS-light-V2 code folder on Kaggle has a new PyTorch template for quick and easy glaucoma detection setup. This model uses the lightweight MobileNetV3 and achieved a test accuracy of 92.6%: https://www.kaggle.com/code/deathtrooper/pytorch-easy-setup-for-glaucoma-detection-92-6
* 03/09/24 : EyePACS-light-V2 now has a 10.0 Kaggle usability score: supplemental metadata.csv file added to dataset.
* 01/20/24 : EyePACS-light-V2 preprocess high-level overview is now available on the Kaggle dataset link in the about section (scroll all the way down) if you are curious on how the dataset was derived
* 12/28/23 : EyePACS-light-V2 94.94% test accuracy benchmark using ConvNeXtTiny: https://www.kaggle.com/code/deathtrooper/benchmark-94-94-convnexttiny
* 12/12/23 : EyePACS-light-V2 is HERE!!! Be the first to benchmark your model with this improved dataset! Download from kaggle: https://www.kaggle.com/datasets/deathtrooper/glaucoma-dataset-eyepacs-airogs-light-v2/data

## Citation Note
If you found this catalog helpful, please consider citing the following:
- Riley Kiefer, Muhammad Abid, Jessica Steen, Mahsa Raeisi Ardali, and Ehsan Amjadian. 2023. A Catalog of Public Glaucoma Datasets for Machine Learning Applications: A detailed description and analysis of public glaucoma datasets available to machine learning engineers tackling glaucoma-related problems using retinal fundus images and OCT images. In Proceedings of the 2023 7th International Conference on Information System and Data Mining (ICISDM '23). Association for Computing Machinery, New York, NY, USA, 24–31. https://doi.org/10.1145/3603765.3603779


# Public Glaucoma Dataset Catalog
[Help expand this repository by providing links/publications to new glaucoma datasets!]

## Repository Table of Contents
- README.md : Glaucoma overview, relevant research, and dataset access links
- benchmark-eyepacs-airogs-light.md : Leaderboard for the test set evaluation using the train/val sets of the EyePACS-AIROGS-light dataset
- summary.md : Dataset class breakdown, image types, and glaucoma types
- data-availability.md : Dataset image and segmentation availability.
- origin.md : Dataset collection origin and collection years.

## Glaucoma Overview
According to AAO, "Glaucoma is a disease that damages your eye’s optic nerve. It usually happens when fluid builds up in the front part of your eye. That extra fluid increases the pressure in your eye, damaging the optic nerve". It is a leading cause of blindness and worsens over time if left untreated. Optometrists diagnose glaucoma through fundus images (a 2D image of the eye) or ocular coherence tomography (OCT) images (a 3D image of the eye). In fundus images, optometrists typically look for optic cup or optic disc damage. In OCT images, optometrists typically look for layer atrophy. To automate the detection of glaucoma, datasets are curated for machine learning. Fundus image datasets are typically designed for either glaucoma classification to distinguish healthy for glaucoma or optic nerve head segmentation to extract and analyze cup or disc damage. High-quality benchmark datasets like EyePACS-AIROGS-light have predetermined train, validation, and test sets for reproducibility.

## Relevant Glaucoma Datasets (by me)
 - SMDG-19 [Dataset], "Standardized Multi-Channel Dataset for Glaucoma, Version 19", https://www.kaggle.com/datasets/deathtrooper/multichannel-glaucoma-benchmark-dataset
 - EyePACS-AIROGS-light-v1 [Dataset], "EyePACS Artificial Intelligence for Robust Glaucoma Screening Challenge, Lightweight Version 1", https://www.kaggle.com/datasets/deathtrooper/eyepacs-airogs-light
 - EyePACS-AIROGS-light-v2 [Dataset], "EyePACS Artificial Intelligence for Robust Glaucoma Screening Challenge, Lightweight Version 2", https://www.kaggle.com/datasets/deathtrooper/glaucoma-dataset-eyepacs-airogs-light-v2

## Relevant Glaucoma Research (by me)
 - ARVO 2024 [Abstract], "Assessment of Retinal Vasculature for Glaucoma Detection: A Comparative Analysis of Human Expertise and Deep Learning Algorithms", https://iovs.arvojournals.org/article.aspx?articleid=2794846
 - AAO 2022 [Abstract], "A Comprehensive Survey of Publicly Available Glaucoma Datasets for Automated Glaucoma Detection", https://aaopt.org/past-meeting-abstract-archives/?SortBy=ArticleYear&ArticleType=&ArticleYear=2022&Title=&Abstract=&Authors=&Affiliation=&PROGRAMNUMBER=225129
 - AAO 2023 [Abstract], "The Predictive Power of Fundus Blood Vessels in Glaucoma Detection", accepted as a presentation for AAO 2023
 - AAO 2023 [Abstract], "EyePACS-light: A Lightweight Balanced Dataset for Automated Glaucoma Classification Modeling", accepted as a poster for AAO 2023 
 - ARVO 2023 [Abstract], "Ground truth validation of publicly available datasets utilized in artificial intelligence models for glaucoma detection", https://iovs.arvojournals.org/article.aspx?articleid=2791017
 - ARVO 2023 [Abstract], "Standardized and Open-Access Glaucoma Dataset for Artificial Intelligence Applications", https://iovs.arvojournals.org/article.aspx?articleid=2790420
 - IEEE-IEMCOM 2022 [Full Paper], "A Survey of Glaucoma Detection Algorithms using Fundus and OCT Images", https://ieeexplore.ieee.org/abstract/document/9946629
 - IEEE-ICIVC 2023 [Full Paper], "Automated Fundus Image Standardization Using a Dynamic Global Foreground Threshold Algorithm", https://ieeexplore.ieee.org/abstract/document/10270429
 - ICISDM 2023 [Full Paper], "A Catalog of Public Glaucoma Datasets for Machine Learning Applications", https://dl.acm.org/doi/abs/10.1145/3603765.3603779

## Example data
Drishti-GS |   G1020 |   ORIGA-light |   REFUGE1-VAL |   PAPILA
--- | --- | --- | --- | ---
<img src="https://user-images.githubusercontent.com/65875562/204176385-9402294e-7b82-4ea3-a1cd-f44e8423ca4f.png" width="128"> |<img src="https://user-images.githubusercontent.com/65875562/204176473-f95150ed-161a-496e-bf44-5af1fa23d736.jpg" width="128"> | <img src="https://user-images.githubusercontent.com/65875562/204176324-eb665daf-60f0-4333-ae77-b78c8e2d038f.jpg" width="128"> | <img src="https://user-images.githubusercontent.com/65875562/204176603-03c21546-2bcf-4e73-b522-ffdacc61ae91.jpg" width="128"> | <img src="https://user-images.githubusercontent.com/65875562/204176775-c4d557c6-ecfc-49a1-a854-b338f5850337.jpg" width="128">

 ## Use Case Acronyms
- Classification
    - BGC = Binary Glaucoma Classification (healthy vs. glaucoma or non-glaucoma vs. glaucoma)
    - MGC = Multi Glaucoma Classification (at least 2 glaucoma types, including suspect)
- Segmentation
    - ODS = Optic Disc Segmentation
    - OCS = Optic Cup Segmentation
    - BVS = Blood Vessel Segmentation
    - OLS = OCT Layer Segmentation
    - RNFLS = Retinal Nerve Fiber Layer Segmentation
- Other
    - LT = Localization Task
    - IQA = Image Quality Assesment
    - MIDI = Multi Image Domain Input
    - CDR = Cup-to-Disc Ratio Estimation
    - N = Notching
    - VF = Visual Field Information/Segmentation
  
## Public Glaucoma Image Datasets
| Dataset   | Access Link | Accessibility | Glaucoma Labels? | Use Case |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| ACRIMA  | https://figshare.com/s/c2d31f850af14c5b5232  | open | Y | BGC |
| AGE  | https://age.grand-challenge.org/Download/  | registration | Y | MGC, LT |
| BEH (Bangladesh Eye Hospital) | https://github.com/mirtanvirislam/Deep-Learning-Based-Glaucoma-Detection-with-Cropped-Optic-Cup-and-Disc-and-Blood-Vessel-Segmentation/tree/master/Dataset | open | Y | BGC |
| BIOMISA | https://data.mendeley.com/datasets/2rnnz5nz74/2  | open | Y | MGC, BGC, MIDI, OLS, CDR |
| Chaksu-IMAGE | https://doi.org/10.6084/m9.figshare.20123135 | open | Y | BGC |
| CRFO-v4 | https://data.mendeley.com/datasets/trghs22fpg/4 | open | Y | BGC, MDI, ODS, OCS |
| DR-HAGIS | https://personalpages.manchester.ac.uk/staff/niall.p.mcloughlin/ | open | Y | BGC, BVS |
| DRIONS-DB  | https://www.researchgate.net/publication/326460478_Glaucoma_dataset_-_DRIONS-DB  | open | N | ODS |
| DRISHTI-GS1  | https://cvit.iiit.ac.in/projects/mip/drishti-gs/mip-dataset2/Home.php  | open | Y | BGC, ODS, OCS, CDR, N |
| EyePACS-AIROGS | https://airogs.grand-challenge.org/data-and-challenge/ | open | Y | BGC, IQA |
| EyePACS-AIROGS-light (v1) | https://www.kaggle.com/datasets/deathtrooper/eyepacs-airogs-light | registration | Y | BGC |
| EyePACS-AIROGS-light (v2) | https://www.kaggle.com/datasets/deathtrooper/glaucoma-dataset-eyepacs-airogs-light-v2 | registration | Y | BGC |
| FIVES | https://figshare.com/articles/figure/FIVES_A_Fundus_Image_Dataset_for_AI-based_Vessel_Segmentation/19688169/1 | open | Y | BGC, BVS |
| G1020 | https://www.kaggle.com/datasets/arnavjain1/glaucoma-datasets | registration | Y | BGC, ODS, OCS |
| GAMMA | https://gamma.grand-challenge.org/ | registration | Y | BGC?, ODS, OCS, OLS?, LT, MIDI |
| GOALS | https://ichallenges.grand-challenge.org/iChallenge-GON3/ | registration | Y | BGC, OLS |
| GRAPE | https://springernature.figshare.com/collections/GRAPE_A_multi-modal_glaucoma_dataset_of_follow-up_visual_field_and_fundus_images_for_glaucoma_management/6406319/1 | open | Y | MGC, VF |
| Harvard-GF | https://ophai.hms.harvard.edu/datasets/harvard-glaucoma-fairness-3300-samples/ | request | N | BGC, VF, RNFLS, MIDI |
| HRF | https://www5.cs.fau.de/research/data/fundus-images/  | open | Y |
| INSPIRE-AVR-test | https://medicine.uiowa.edu/eye/inspire-datasets | open | N |
| INSPIRE-STEREO | https://medicine.uiowa.edu/eye/inspire-datasets | open | N |
| JSIEC-1000 | https://www.kaggle.com/datasets/linchundan/fundusimage1000 | registration | Y |
| KEH (Kim's Eye Hospital) | https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/1YRRAC | open | Y |
| LAG | https://github.com/smilell/AG-CNN | request | Y |
| LES-AV | https://figshare.com/articles/dataset/LES-AV_dataset/11857698/1 | open | Y |
| Leuven-Haifa HRF | https://rdr.kuleuven.be/dataset.xhtml?persistentId=doi:10.48804/Z7SHGO | request | Y | MGC, BVS |
| MSHF | https://www.nature.com/articles/s41597-023-02188-x#ref-CR17 | open | Y | BGC, IQA |
| OCTV | https://zenodo.org/record/1481223#.Y20g3XbMIuV | open | Y |
| OIA-ODIR | https://www.kaggle.com/datasets/andrewmvd/ocular-disease-recognition-odir5k | registration | Y |
| ONHSD | https://aldiri.info/Image%20Datasets/ONHSD.aspx | inaccessible | Y |
| ORIGA-light | https://www.kaggle.com/datasets/sshikamaru/glaucoma-detection | registration | Y |
| PAPILA | https://doi.org/10.6084/m9.figshare.14798004.v1 | open | Y |
| REFUGE1  | https://refuge.grand-challenge.org/REFUGE2Download/  | registration | Y |
| REFUGE2  | https://refuge.grand-challenge.org/REFUGE2Download/  | registration | Y |
| RIGA-BIN-RUSHED | https://deepblue.lib.umich.edu/data/concern/data_sets/3b591905z  | open | N |
| RIGA-MAGRABI | https://deepblue.lib.umich.edu/data/concern/data_sets/3b591905z  | open | N |
| RIGA-MESSIDOR | https://deepblue.lib.umich.edu/data/concern/data_sets/3b591905z  | open | N |
| RIM-ONE-r1 | http://medimrg.webs.ull.es/research/retinal-imaging/rim-one/  | open | Y |
| RIM-ONE-r2 | http://medimrg.webs.ull.es/research/retinal-imaging/rim-one/  | open | Y |
| RIM-ONE-r3 | http://medimrg.webs.ull.es/research/retinal-imaging/rim-one/  | open | Y |
| RIM-ONE-DL | http://medimrg.webs.ull.es/research/retinal-imaging/rim-one/  | open | Y |
| SIGF | https://github.com/XiaofeiWang2018/DeepGF | request | Y |
| SMDG | https://www.kaggle.com/datasets/deathtrooper/multichannel-glaucoma-benchmark-dataset | registration | Y |
| sjchoi86-HRF | https://github.com/yiweichen04/retina_dataset | open | Y |
| VEIRC | https://github.com/ProfMKD/Glaucoma-dataset | open | Y |
