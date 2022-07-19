# multichannel-glaucoma-benchmark-dataset
Public multi-channel benchmark dataset for Glaucoma classification.

## Cite this dataset
- *INSERT CITATION HERE*

## Objective
The objective of this glaucoma benchmark dataset is to compile all available public glaucoma datasets into a single large dataset. This dataset will standardize image metadata and multi-modal image/segmentation data into machine-learning-ready data. Additionally, the benchmark dataset will provide dataset-level metadata related to the image collection study for metadata analysis. All dataset instances have the following linking constraint: the optic nerve head cropped fundus image. 

## Data Access Link
https://www.kaggle.com/datasets/deathtrooper/multichannel-glaucoma-benchmark-dataset

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
- KEH

## Pending Datasets
- BIOMISA
- INSPIRE-stereo
- INSPIRE-AVR
- RIM-ONE-r1 (other versions do not differentiate glaucoma vs glaucoma suspect)
- EyePACS-AIROGS

## Benchmark Dataset File Structure
- Glaucoma Suspect (-1)
  - Glaucoma Suspect Instance 1
    - channel image data (fundus, oct, optic disc, ...)
  - ...
- Glaucoma (1)
  - Glaucoma Instance 1
    - channel image data (fundus, oct, optic disc, ...)
  - ...
- Healthy (0)
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
- Types: Majority Consensus of the Glaucoma classification; 0 = healthy, -1 = glaucoma suspect; 1 = glaucoma
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
- expert1_grade: Glaucoma classification from expert 1; 0 = healthy, -1 = glaucoma suspect; 1 = glaucoma
- expert2_grade: Glaucoma classification from expert 2; 0 = healthy, -1 = glaucoma suspect; 1 = glaucoma
- expert3_grade: Glaucoma classification from expert 3; 0 = healthy, -1 = glaucoma suspect; 1 = glaucoma
- expert4_grade: Glaucoma classification from expert 4; 0 = healthy, -1 = glaucoma suspect; 1 = glaucoma
- expert5_grade: Glaucoma classification from expert 5; 0 = healthy, -1 = glaucoma suspect; 1 = glaucoma
- cdr_avg: Average CDR estimation from all experts
- cdr_expert1: CDR estimation from expert 1
- cdr_expert2: CDR estimation from expert 2
- cdr_expert3: CDR estimation from expert 3
- cdr_expert4: CDR estimation from expert 4
- glaucoma_type: Expert diagnoisis of glaucoma subtype (ex. early glaucoma, advanced glaucoma, open angle, closed angle, ...)

## Original Public Dataset Sources and Citations
- ACRIMA
  - URL: https://figshare.com/s/c2d31f850af14c5b5232
  - LaTex: @article{arcima,
  title={CNNs for automatic glaucoma assessment using fundus images: an extensive validation},
  author={Diaz-Pinto, Andres and Morales, Sandra and Naranjo, Valery and K{\"o}hler, Thomas and Mossi, Jose M and Navea, Amparo},
  journal={Biomedical engineering online},
  volume={18},
  number={1},
  pages={1--19},
  year={2019},
  publisher={Springer}
}
- DRISHTI-GS1
  - URL: https://cvit.iiit.ac.in/projects/mip/drishti-gs/mip-dataset2/Home.php
  - LaTex: @inproceedings{drishti,
  title={Drishti-gs: Retinal image dataset for optic nerve head (onh) segmentation},
  author={Sivaswamy, Jayanthi and Krishnadas, SR and Joshi, Gopal Datt and Jain, Madhulika and Tabish, A Ujjwaft Syed},
  booktitle={2014 IEEE 11th international symposium on biomedical imaging (ISBI)},
  pages={53--56},
  year={2014},
  organization={IEEE}
}
- HRF
  - URL: https://www5.cs.fau.de/research/data/fundus-images/
  - LaTex: @article{hrf,
  title={Robust vessel segmentation in fundus images},
  author={Budai, Attila and Bock, R{\"u}diger and Maier, Andreas and Hornegger, Joachim and Michelson, Georg},
  journal={International journal of biomedical imaging},
  volume={2013},
  year={2013},
  publisher={Hindawi}
}
- REFUGE1
  - URL: https://refuge.grand-challenge.org/REFUGE2Download/
  - LaTex: @article{refuge,
  title={Refuge challenge: A unified framework for evaluating automated methods for glaucoma assessment from fundus photographs},
  author={Orlando, Jos{\'e} Ignacio and Fu, Huazhu and Breda, Jo{\~a}o Barbosa and van Keer, Karel and Bathula, Deepti R and Diaz-Pinto, Andr{\'e}s and Fang, Ruogu and Heng, Pheng-Ann and Kim, Jeyoung and Lee, JoonHo and others},
  journal={Medical image analysis},
  volume={59},
  pages={101570},
  year={2020},
  publisher={Elsevier}
}
- RIM-ONE
  - URL: http://medimrg.webs.ull.es/research/retinal-imaging/rim-one/
  - LaTex: @inproceedings{rim-one,
  title={RIM-ONE: An open retinal image database for optic nerve evaluation},
  author={Fumero, Francisco and Alay{\'o}n, Silvia and Sanchez, Jos{\'e} L and Sigut, Jose and Gonzalez-Hernandez, M},
  booktitle={2011 24th international symposium on computer-based medical systems (CBMS)},
  pages={1--6},
  year={2011},
  organization={IEEE}
}
- RIM-ONE-DL
  - URL: http://medimrg.webs.ull.es/research/retinal-imaging/rim-one/
  - LaTex: @article{rim-one-dl,
  title={RIM-ONE DL: A Unified Retinal Image Database for Assessing Glaucoma Using Deep Learning},
  author={Batista, Francisco Jos{\'e} Fumero and Diaz-Aleman, Tinguaro and Sigut, Jose and Alayon, Silvia and Arnay, Rafael and Angel-Pereira, Denisse},
  journal={Image Analysis \& Stereology},
  volume={39},
  number={3},
  pages={161--167},
  year={2020}
}
- BIOMISA
  - URL: https://data.mendeley.com/datasets/2rnnz5nz74/2
  - LaTex: @article{biomisa,
  title={Data on OCT and fundus images for the detection of glaucoma},
  author={Raja, Hina and Akram, M Usman and Khawaja, Sajid Gul and Arslan, Muhammad and Ramzan, Aneeqa and Nazir, Noman},
  journal={Data in brief},
  volume={29},
  pages={105342},
  year={2020},
  publisher={Elsevier}
}
- DR-HAGIS
  - URL: https://personalpages.manchester.ac.uk/staff/niall.p.mcloughlin/
  - LaTex: @article{drhagis,
  title={DR HAGIS—a fundus image database for the automatic extraction of retinal surface vessels from diabetic patients},
  author={Holm, Sven and Russell, Greg and Nourrit, Vincent and McLoughlin, Niall},
  journal={Journal of Medical Imaging},
  volume={4},
  number={1},
  pages={014503},
  year={2017},
  publisher={SPIE}
}
- OIA-ODIR
  - URL: https://www.kaggle.com/datasets/andrewmvd/ocular-disease-recognition-odir5k
  - LaTex: @inproceedings{odir,
  title={A benchmark of ocular disease intelligent recognition: one shot for multi-disease detection},
  author={Li, Ning and Li, Tao and Hu, Chunyu and Wang, Kai and Kang, Hong},
  booktitle={International Symposium on Benchmarking, Measuring and Optimization},
  pages={177--193},
  year={2020},
  organization={Springer}
}
- JSIEC-1000
  - URL: https://www.kaggle.com/datasets/linchundan/fundusimage1000
  - LaTex: @article{jsiec,
  title={Automatic detection of 39 fundus diseases and conditions in retinal photographs using deep neural networks},
  author={Cen, Ling-Ping and Ji, Jie and Lin, Jian-Wei and Ju, Si-Tong and Lin, Hong-Jie and Li, Tai-Ping and Wang, Yun and Yang, Jian-Feng and Liu, Yu-Fen and Tan, Shaoying and others},
  journal={Nature communications},
  volume={12},
  number={1},
  pages={1--13},
  year={2021},
  publisher={Nature Publishing Group}
}
- sjchoi86-HRF
  - URL: https://github.com/cvblab/retina_dataset
  - LaTex: @misc{sjchoi86,
    title={sjchoi86-HRF Database},
    author={S. Choi},
    note={Link : \url{http://github.com/yiweichen04/retina_dataset}}
}
- CRFO-v4
  - URL: https://data.mendeley.com/datasets/trghs22fpg/4
  - LaTex: N/A
- BEH (Bangladesh Eye Hospital)
  - URL: https://github.com/mirtanvirislam/Deep-Learning-Based-Glaucoma-Detection-with-Cropped-Optic-Cup-and-Disc-and-Blood-Vessel-Segmentation/tree/master/Dataset
  - LaTex: @article{BEH,
  author={Islam, Mir Tanvir and Mashfu, Shafin T. and Faisal, Abrar and Siam, Sadman Chowdhury and Naheen, Intisar Tahmid and Khan, Riasat},
  journal={IEEE Access}, 
  title={Deep Learning-Based Glaucoma Detection With Cropped Optic Cup and Disc and Blood Vessel Segmentation}, 
  year={2022},
  volume={10},
  number={},
  pages={2828-2841},
  doi={10.1109/ACCESS.2021.3139160}}
- ORIGA-light
  - URL: https://www.kaggle.com/datasets/sshikamaru/glaucoma-detection
  - LaTex: @inproceedings{origa,
  title={Origa-light: An online retinal fundus image database for glaucoma analysis and research},
  author={Zhang, Zhuo and Yin, Feng Shou and Liu, Jiang and Wong, Wing Kee and Tan, Ngan Meng and Lee, Beng Hai and Cheng, Jun and Wong, Tien Yin},
  booktitle={2010 Annual International Conference of the IEEE Engineering in Medicine and Biology},
  pages={3065--3068},
  year={2010},
  organization={IEEE}
}
- LES-AV
  - URL: https://figshare.com/articles/dataset/LES-AV_dataset/11857698/1
  - LaTex: @inproceedings{lesav,
  title={Towards a glaucoma risk index based on simulated hemodynamics from fundus images},
  author={Orlando, Jos{\'e} Ignacio and Barbosa Breda, Jo{\~a}o and Keer, Karel van and Blaschko, Matthew B and Blanco, Pablo J and Bulant, Carlos A},
  booktitle={International Conference on Medical Image Computing and Computer-Assisted Intervention},
  pages={65--73},
  year={2018},
  organization={Springer}
}
- KEH (Kim's Eye Hospital)
  - URL: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/1YRRAC
  - LaTex: @data{DVN/1YRRAC_2018,
  author = {Kim, Ungsoo},
  publisher = {Harvard Dataverse},
  title = {{Machine learn for glaucoma}},
  year = {2018},
  version = {V1},
  doi = {10.7910/DVN/1YRRAC},
  url = {https://doi.org/10.7910/DVN/1YRRAC}
}
