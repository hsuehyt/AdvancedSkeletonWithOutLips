# AdvancedSkeleton Without Lips

This repository contains a customized version of the **AdvancedSkeleton** rigging toolset for Autodesk Maya, specifically modified to bypass lip controls for characters without lips. This version of the tool allows users to rig facial features that do not require lip joints while maintaining other AdvancedSkeleton functionalities.

## Features
- Lip controls (e.g., `FaceFitLipOuter`, `FaceFitLipMain`, `FaceFitLipInner`) are bypassed.
- Suitable for rigging characters that lack lips or have simplified mouth structures.
- Maintains the core AdvancedSkeleton functionality for facial rigging (eyes, jaw, cheeks, etc.).
- No more errors related to missing lip geometry during the rigging process.

## Installation

1. Download or clone this repository.

2. Copy the modified `AdvancedSkeleton.mel` script to replace the original one under your **AdvancedSkeleton** folder:

   ![AdvancedSkeleton Folder Location](https://github.com/hsuehyt/AdvancedSkeletonWithOutLips/blob/main/README/Screenshot%202024-10-27%20155122.png)

3. In Maya, source the script to load AdvancedSkeleton as you normally would.

4. Follow the regular workflow for using AdvancedSkeleton, without worrying about lip controls.

## Usage

- After installing the modified script, you can use AdvancedSkeleton to rig faces as usual, but the script will no longer expect or require lip joints during the **FitSkeleton** or **FaceSetup** phases.
- Other facial controls, such as those for the eyes, cheeks, and jaw, remain functional.
  
## Modifications

The following changes were made to the original **AdvancedSkeleton.mel** script:
- Lip-related controls (`FaceFitLipOuter`, `FaceFitLipMain`, `FaceFitLipInner`, and their associated selections) were commented out.
- The script logic was adjusted to prevent any errors related to missing lips during rig creation.

## Known Issues
- Ensure all other required controls (e.g., for eyes, jaw) are set up properly to avoid rigging issues.
- If your character design changes and requires lips later, revert to the original AdvancedSkeleton version.

## License
This project follows the same licensing terms as the original **AdvancedSkeleton** toolset. Please refer to [AdvancedSkeleton License](https://animationstudios.com.au/advanced-skeleton-download/) for more details.