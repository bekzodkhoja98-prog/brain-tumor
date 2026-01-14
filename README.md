# brain-tumor (MONAI studies)

This repository contains MRI studies prepared for MONAI/MONAI Label.

## Structure
Each patient is split into zip parts because of GitHub upload limits.

After downloading all parts, extract them into the same folder. Final structure should be:

MONAI_STUDIES/
  Patient_0001/images/*.nii.gz
  Patient_0002/images/*.nii.gz
  ...

## How to run MONAI Label
Example:
monailabel start_server --app radiology --studies D:\MONAI_STUDIES --port 8000

## Notes
- Files are anonymized (Patient_0001, Patient_0002, etc.)
- manifest.json contains mapping from DICOM series to NIfTI outputs.
