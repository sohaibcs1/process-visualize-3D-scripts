# process-visualize-3D
Python toolkit to process, analyze, and visualize 3D medical and scientific image data. Supports formats like NIfTI, VTP, and TIFF, with integration for VTK, connected components, and Matplotlib. Ideal for segmentation, rendering, and volumetric exploration.


## 📄 Notebooks Overview

- **`3Dnii_apply_custom_cellColor_pyqt.ipynb`**  
  Interactive PyQt5-based application for visualizing connected components in a 3D NIfTI segmentation volume.  
  Allows users to assign custom colors to each segmented component and switch between multiple 3D views (top, side, front, isometric).  
  Uses VTK for real-time rendering and `cc3d` for connected component labeling.

- **`nii_animate_and_Savevideo.ipynb`**  
  Loads 3D segmentation masks (NIfTI format), extracts connected components, and renders them in 3D using VTK.  
  Applies custom spatial positioning and camera rotation to create a composite scene of multiple samples.  
  Captures the rotating 3D visualization as a video and saves it using OpenCV.

- **`nii_applyConnectedComponent_render.ipynb`**  
  Loads a 3D segmentation NIfTI file and applies connected component labeling using `cc3d`.  
  Visualizes the labeled components as 3D surfaces using VTK’s Discrete Marching Cubes and smoothing filters.  
  Assigns random colors to each component and provides an interactive 3D view with axes and custom camera setup.
