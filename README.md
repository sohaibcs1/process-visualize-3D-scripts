# process-visualize-3D
Python toolkit to process, analyze, and visualize 3D medical and scientific image data. Supports formats like NIfTI, VTP, and TIFF, with integration for VTK, connected components, and Matplotlib. Ideal for segmentation, rendering, and volumetric exploration!@


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
  
- **`read_meta_czi (1).ipynb`**  
  Extracts and displays metadata from `.czi` microscopy image files using the Bio-Formats library.  
  Retrieves channel information such as the number of channels and their names from OME-XML metadata.  
  Useful for verifying channel structure before image processing or analysis.

- **`blob_detection_log.ipynb`**  
  Detects circular features (cells or blobs) in grayscale images using the Laplacian of Gaussian (LoG) method.  
  Applies contrast stretching for preprocessing and visualizes detected blobs using `matplotlib`.  
  Returns the total count and coordinates of all detected blobs, useful for cell quantification tasks.

- **`cellLine_analysis_violin_pca_tsne.ipynb`**  
  Performs exploratory analysis on cellular feature data by generating violin plots with statistical significance (Mann-Whitney U test).  
  Extracts cell line and day information for group comparisons and visualizes feature distributions.  
  Applies PCA and t-SNE for dimensionality reduction to visualize clustering patterns across cell lines.

- **`czi_to_nii.ipynb`**  
  Converts `.czi` and other microscopy file formats into `.nii.gz` (NIfTI) using the Bio-Formats library.  
  Supports multi-channel and volumetric microscopy data with metadata handling.  
  Ideal for preparing raw experimental files for downstream 3D processing and deep learning pipelines.



