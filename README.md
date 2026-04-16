# Collecting System, Calcium Oxalate and Uric Acid Stone Digital Renderings

A high-fidelity, open-source 3D digital twin of the renal collecting system and kidney stones designed for simulated ureteroscopy and the training of computer vision models.

---

## ## Overview

While surgical simulation is a vital tool for medical education, there is a current lack of open-source 3D models featuring highly realistic textures of the renal collecting system or common calculi. 

We addresses this gap by providing a virtual representation validated by endourologists for both textural and geometric accuracy. These assets serve as the foundation for:
* **Digital Surgical Scenes:** Training vision models to enable computer-assisted surgery.
* **Realistic Digital Trainers:** Allowing trainees to refine endoscopic techniques without the costs and burdens of physical simulation.

## ## Features

* **Validated High-Fidelity Models:** Geometric accuracy optimized for simulated ureteroscopy.
* **Realistic Texturing:** Includes custom HDR and JPEG textures to replicate the endoscopic appearance of the kidney and stones.
* **Multi-Format Support:** Files provided in `.blend`, `.stl`, and Universal Scene Description (`.usd`, `.usda`, `.usdc`) formats for compatibility across Blender, CAD software, and NVIDIA Omniverse/Isaac Gym.

---

## ## Repository Structure

```text
├── kidney-blend-stl-files/
│   ├── smoother-laplace-kidney_model_new.blend  # Source Blender file
│   └── smoother-laplace-kidney_model_new.stl    # Standard Tessellation Language file
├── kidney-files/
│   ├── smoother-laplace-kidney_model_new.usd    # Binary USD file
│   ├── smoother-laplace-kidney_model_new.usda   # ASCII USD file
│   └── smoother-laplace-kidney_model_new.usdc   # Crate (binary) USD file
├── texture/
│   ├── color_121212.hdr                         # High Dynamic Range environment/color map
│   ├── kidney_texture.jpg                       # Primary kidney surface texture
│   └── texture_new.jpg                          # Updated texture assets
└── blank.txt                                    # Placeholder/Initialization file
```

## ## Getting Started

### ### Prerequisites
To view and manipulate the models, it is recommended to use:
* **Blender** (for `.blend` and texturing)
* **NVIDIA Omniverse** (for `.usd` workflows and AI training)
* **MeshLab** (for `.stl` inspection)

### ### Usage
1. Clone the repository:
   `git clone https://github.com/[username]/uro-glidar.git`
2. Import the desired model from the `kidney-files` or `kidney-blend-stl-files` directory into your simulation environment.
3. Apply textures from the `texture/` folder to the mesh to achieve validated endoscopic realism.

---

## ## Implications
Accurately replicating surgical anatomy is the first step in creating autonomous or assisted surgical pipelines. By providing these high-fidelity assets open-source, we aim to accelerate the development of endourologic AI and simulation-based training.

How would you like to handle the licensing section for this—should we stick with a standard MIT or a Creative Commons Attribution?
