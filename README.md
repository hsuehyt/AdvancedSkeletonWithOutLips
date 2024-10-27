# AdvancedSkeleton Without Lips

This repository contains a customized version of the **AdvancedSkeleton** rigging toolset for Autodesk Maya, specifically modified to bypass lip and related facial controls for characters without lips. This version allows users to rig facial features while excluding areas such as lips, cheeks, jaw, and nose.

## Features
- Lip controls (e.g., `FaceFitLipOuter`, `FaceFitLipMain`, `FaceFitLipInner`) are bypassed.
- The rigging will **lose functionality** for facial areas that are typically controlled by lip joints, including:
  - **Lips**
  - **Cheeks**
  - **Jaw**
  - **Nose**
- This version is suitable for characters that don't need detailed facial expressions involving these features.

## Installation

1. Download or clone this repository.

2. Copy the modified `AdvancedSkeleton.mel` script to replace the original one under your **AdvancedSkeleton** folder:

   ![AdvancedSkeleton Folder Location](https://github.com/hsuehyt/AdvancedSkeletonWithOutLips/blob/main/README/Screenshot%202024-10-27%20155122.png)

3. In Maya, source the script to load AdvancedSkeleton as you normally would.

4. Follow the regular workflow for using AdvancedSkeleton, but be aware that controls for lips, cheeks, jaw, and nose will no longer be available.

## Usage

- After installing the modified script, you can use AdvancedSkeleton to rig faces as usual. However, the script will no longer expect or require lip joints during the **FitSkeleton** or **FaceSetup** phases.
- **Important:** The loss of lip joints also affects the functionality of other related facial features. As a result, movements for the **nose**, **jaw**, and **cheeks** will not work as expected.

## Modifications

The following changes have been made based on AdvancedSkeleton Version 6.400:
- Lip-related controls (`FaceFitLipOuter`, `FaceFitLipMain`, `FaceFitLipInner`, and their associated selections) were commented out.
- Nose, jaw, and cheek movements were affected due to the exclusion of these controls.
- The script logic was adjusted to prevent any errors related to missing lip joints during rig creation.

## Known Issues
- Ensure all other required controls (e.g., for eyes) are set up properly to avoid rigging issues.
- If your character design changes and requires detailed facial movements later, including the nose, cheeks, jaw, or lips, revert to the original AdvancedSkeleton version.

## License
This project follows the same licensing terms as the original **AdvancedSkeleton** toolset. Please refer to [AdvancedSkeleton License](https://animationstudios.com.au/advanced-skeleton-download/) for more details.