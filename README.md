# Protein Structure Prediction using AlphaFold 3

This repository contains a portfolio project showcasing the 3D structure prediction of a target protein using Google DeepMind's **AlphaFold 3**. This project demonstrates the practical applications of Artificial Intelligence (AI) and Machine Learning in Structural Biology.

## 🧬 Project Overview
- **Prediction Tool:** AlphaFold 3
- **Platform used:** Google Colab
- **Target Protein Length:** 417 Residues (Chain A)

### Predicted 3D Structure Visualization
Below is the 3D ribbon model of the predicted protein structure visualized using Mol* Viewer:

![Predicted Protein Structure](protein_model.png)

---

## 📊 Model Quality & Confidence Metrics
AlphaFold 3 evaluates its own structural predictions using specific confidence scores. Based on the generated `summary_confidence_0.json` file, the model metrics are highly reliable:

- **Overall Confidence:** The structural core is predicted with exceptional accuracy, showing local confidence scores tracking well above **95.0** (peaking around 98.7).
- **Flexible Regions:** The model successfully identified highly flexible loop regions (around residues 50-65 and 240-245) and a highly disordered C-terminus tail where the confidence score dropped naturally, reflecting real biological flexibility.

---

## 📂 Repository Structure
- `fold_2026_06_11_15_58_model_0.cif` - The main 3D coordinate file containing the highest-ranked predicted model.
- `fold_2026_06_11_15_58_summary_confidence_0.json` - Complete metadata containing quality metrics, pLDDT scores, and predicted alignment errors.
- `msas/` - Folder containing the Multiple Sequence Alignments used by AlphaFold to study the evolutionary history of the protein.
- `protein_model.png` - Captured 3D snapshot of the predicted model.

---

## 🛠️ How to View the 3D Model Locally
1. Download the `.cif` file from this repository.
2. Open your browser and go to [Mol* Viewer](https://www.rcsb.org/3d-view) or [Molstar Org](https://molstar.org/viewer/).
3. Click on **Open Files** and upload the downloaded `.cif` file to interact with the 3D protein structure.
