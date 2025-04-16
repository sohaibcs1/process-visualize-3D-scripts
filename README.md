# process-visualize-3D
Python toolkit to process, analyze, and visualize 3D medical and scientific image data. Supports formats like NIfTI, VTP, and TIFF, with integration for VTK, connected components, and Matplotlib. Ideal for segmentation, rendering, and volumetric exploration.


## 📄 Notebooks Overview

### `3Dnii_apply_custom_cellColor_pyqt.ipynb`
Interactive PyQt5-based application for visualizing connected components in a 3D NIfTI segmentation volume.  
Allows users to assign custom colors to each segmented component and switch between multiple 3D views (top, side, front, isometric).  
Uses VTK for real-time rendering and `cc3d` for connected component labeling.
