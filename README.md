# Annular Flow of PTT Fluid - CFD Model

## 👨‍🔬 Author Information

**Taha Rezaee**  
📧 **Email:** [rezaee.taha@gmail.com](mailto:rezaee.taha@gmail.com)  |  🔬 **ORCID:** [![ORCID](https://img.shields.io/badge/ORCID-A6CE39?logo=orcid&logoColor=white)](https://orcid.org/0009-0008-6807-0765)

---

This repository contains Computational Fluid Dynamics (CFD) model files for simulating annular flow development of a Phan-Thien-Tanner (PTT) fluid. The model focuses on the hydrodynamic development region and viscoelastic stress development in annular geometries.

## 📖 Associated Publication

This model is associated with the following scientific publication:

**Rezaee, T.** (2025). Viscoelastic annular entry flow with wall slip: A numerical study of velocity and stress development. *Physics of Fluids*. [![DOI](https://img.shields.io/badge/DOI-10.1063/5.0304570-blue)](https://doi.org/10.1063/5.0304570)
 

## 🚀 Model Specifications

- **Physics:** Viscoelastic fluid flow in annular geometry
- **Fluid Model:** Phan-Thien-Tanner (PTT) constitutive equation
- **Mesh:** Medium-resolution mesh as described in the associated manuscript
- **Geometry:** Annular flow configuration
- **System Requirements:** Minimum of **16 GB RAM** required to run the simulation
- **Software:** COMSOL Multiphysics

## 📁 Repository Contents

- COMSOL model file (.mph) for annular PTT flow simulation
- Documentation files
- Parameter specifications

## ⚠️ CRITICAL IMPLEMENTATION NOTES

**Please Read Carefully Before Use**

### 🎯 Important Limitations & Requirements

**Current Model Scope:**
- This base model file is configured for Deborah numbers **De < 5**
- Validated for moderate viscoelastic parameters
- Uses standard mesh configuration as described in our publication

**For Extended Parameter Ranges:**
To simulate higher Deborah numbers (De > 5) or lower β parameters, the following modifications are **ESSENTIAL**:

1. **Geometry Extension:** Duplicate the outlet block multiple times to ensure full stress development
2. **Mesh Refinement:** Adjust mesh density appropriately for convergence
3. **Convergence Monitoring:** Carefully monitor stress field convergence in extended domains

### 🔬 Technical Justification

The need for geometry extension stems from fundamental viscoelastic flow characteristics:
- Higher De flows require longer development lengths for stress field stabilization
- Inadequate domain length can lead to unphysical results and convergence issues
- These requirements are well-established in viscoelastic CFD literature

### 📝 Important Clarification Regarding Model Files

**Please Note:** Due to the substantial file sizes of comprehensive COMSOL models and associated mesh files, this repository contains the essential model file rather than all possible variations. 

**This is standard practice in computational fluid dynamics** for the following reasons:

- COMSOL files with detailed meshes can exceed multiple GB in size
- Repository limitations prevent hosting all possible parameter variations
- **Researchers experienced in CFD and viscoelastic flows will understand** how to appropriately extend the domain and refine the mesh for their specific parameter ranges
- The provided model serves as a validated foundation that can be adapted as needed

### 🛠️ For CFD Practitioners

Researchers with CFD background should:
- Assess required domain length based on their specific De and β parameters
- Implement appropriate mesh refinement strategies
- Perform convergence studies for extended parameter ranges
- Refer to viscoelastic flow literature for domain length guidelines

## 🤝 Citation and Usage

If you use this model in your research, please cite the associated publication once available. The model is provided to support reproducibility and further research in viscoelastic fluid mechanics.

---

**Disclaimer:** This model is provided as-is for research purposes. Users are expected to have sufficient CFD background to understand the necessary modifications for different parameter regimes, particularly regarding domain length requirements for high Deborah number flows.
