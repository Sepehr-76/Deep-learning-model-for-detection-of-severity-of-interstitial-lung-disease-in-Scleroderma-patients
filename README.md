# Deep learning model for detection of severity of interstitial lung disease in Scleroderma patients

## Task
Scleroderma patients with Interstitial lung disease (ILD) may have different patterns of lung involvement in their CT scan. For the treatment and prognosis assessment of these patients, it is crucial to know the type and severity of the ILD. Currently, radiologists and pulmonologists are required to assess the chest CT scans of these patients, however, an automated process may hopefully reduce their workload. Therefore, in this ongoing project, we aimed to assess the type and percentage of lung disease using the Seg-Res-net model.

## Data
We extracted the CT scans of the patients from the EHR of a tertiary hospital. All chest CT scans were converted to the Nifti file format. A total of 60 chest CT scans are planned to be used in this project.

## Methods

Nifti files were segmented using  3D-slicer application under the supervision of expert radiologists. Next, CT images and labels were pre-processed. We used random Guassian noise, random intensity scaling, and random contrast adjustment for image augmentation. Each CT image has 3 labels (1. ground glass opacity (GGO), 2. Fibrosis, 3. Normal lung). Lung involvement was assessed by the following formula: 

GGO (%)= number of GGO voxels/(number of GGO voxels + number of fibrosis voxels + number of normal lung voxels)

Fibrosis (%)= number of fibrosis voxels/(number of GGO voxels + number of fibrosis voxels + number of normal lung voxels)

Total ILD (%)= (number of GGO voxels + number of fibrosis voxels)/(number of GGO voxels + number of fibrosis voxels + number of normal lung voxels)




## Results

We are waiting for the segmentation process to finish to update the result section.

