# Human Representations in 3D Data Analysis

This project explores multiple ways of representing the human body in computer vision and 3D data analysis workflows. It combines **skeleton-based representations**, **2D/3D human pose estimation**, and **mesh-based geometry analysis** in a single hands-on notebook.

The notebook demonstrates how human motion and shape can be modeled, visualized, and analyzed using modern Python tools such as **MediaPipe**, **OpenCV**, **Matplotlib**, **Plotly**, and **Trimesh**.

## Project Overview

The project is divided into two main parts:

### 1. Skeleton and Pose-Based Human Representation
This part focuses on lightweight human representations built from joints and bones.

It includes:
- Simple 3D skeleton visualization
- Synthetic skeleton motion generation and animation
- 2D human pose estimation from an image using **MediaPipe**
- 3D landmark extraction and interactive pose visualization
- A video-processing template for extending pose estimation to sequences

### 2. Mesh-Based Human Representation
This part explores surface-based 3D representations using polygonal meshes.

It includes:
- Loading and visualizing `.obj` meshes
- Basic geometric inspection of 3D models
- Height-based mesh visualization
- Surface area and volume analysis
- A starting point for comparing different poses using per-vertex displacement

## Repository Structure

```text
.
├── hands_on_human_representations.ipynb
├── README.md
└── requirements.txt
```

## Technologies Used

- Python
- NumPy
- Matplotlib
- OpenCV
- MediaPipe
- Plotly
- Trimesh
- ipywidgets
- Jupyter Notebook

## Installation

Clone the repository and install the dependencies:

```bash
git clone <your-repository-url>
cd <your-repository-folder>
pip install -r requirements.txt
```

Then launch Jupyter:

```bash
jupyter notebook
```

Open:

```text
hands_on_human_representations.ipynb
```

## How to Use

### Skeleton and pose estimation
For the pose-estimation section:
1. Place an input image in the project directory.
2. Rename it or update the notebook path accordingly (the notebook currently expects `img.jpg`).
3. Run the notebook cells in order.

### Mesh analysis
For the mesh-analysis section:
1. Use a valid `.obj` file.
2. Load or upload the mesh as indicated in the notebook.
3. Run the visualization and analysis cells.

## Example Inputs

- A human image for 2D/3D pose estimation
- A `.obj` mesh file for 3D geometry inspection

## Key Learning Outcomes

This project demonstrates:
- The difference between **skeleton-based** and **mesh-based** human representations
- How 2D observations can be transformed into structured pose landmarks
- How to visualize motion and body structure in 3D
- How to inspect and analyze mesh geometry programmatically

## Notes

- Some cells were originally written with notebook/Colab-style installation commands.
- The mesh upload utility uses a Colab-oriented workflow in one section. If you run this locally, you may want to replace the upload step with direct local file loading.
- MediaPipe 3D landmarks are estimated relative to the detected pose and are useful for visualization, but they are not equivalent to metrically accurate full-body reconstruction.

## Possible Improvements

Future extensions could include:
- Support for local file pickers instead of Colab upload utilities
- Processing full videos for temporal pose analysis
- Using SMPL or similar parametric body models
- Comparing multiple meshes across poses or identities
- Exporting animations and plots automatically

## Author

Mahmoud Abo Shukr

## License

This repository is shared as a personal academic project and portfolio item. Add a license file if you want to define reuse permissions explicitly.
