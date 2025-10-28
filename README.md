# 🧬 PRMT5_IntegrativeAnalysis  
### Structural Mechanisms and Molecular Insights into PRMT5 Inhibition

Welcome to the official repository for our computational study on **Protein Arginine Methyltransferase 5 (PRMT5)** — a key enzyme involved in histone arginine methylation and RNA splicing.  
This project integrates **machine learning-based QSAR modeling**, **molecular docking**, **molecular dynamics (MD) simulations**, and **network pharmacology analysis** to uncover the molecular basis of PRMT5 inhibition and identify promising inhibitor candidates.

---

## 📘 Overview
PRMT5 plays an essential role in chromatin regulation and RNA processing. Its overexpression has been linked to multiple cancers, including glioblastoma, lung carcinoma, and MTAP-deleted tumors.  
Targeting PRMT5 offers a strategy for selective cancer therapy by blocking its methyltransferase activity.

This repository provides all curated data, scripts, and analysis outputs used to:
- Predict and validate potent PRMT5 inhibitors.  
- Examine ligand stability and conformational behavior via MD simulations.  
- Explore functional gene networks and pathways associated with PRMT5 inhibition.

---

## ⚙️ Methodology

### 🧩 1. Data Curation  
- PRMT5 inhibitor data retrieved from the **ChEMBL** database.  
- Duplicates and incomplete entries removed; IC₅₀ values converted to pIC₅₀.  
- Descriptors generated using **PubChem**, **MACCS**, **Substructure**, and **Klekota-Roth** fingerprints.

### 🤖 2. Machine Learning Models  
- Models built with **Random Forest (RF)**, **Support Vector Regression (SVR)**, **Kernel Ridge Regression (KRR)**, and **XGBoost (XGB)**.  
- Feature interpretability assessed using **SHAP** values, **PCA**, and **entropy-based diversity**.  
- Model validation followed OECD guidelines (R², RMSE, CCC, and Y-randomization).

### 🧬 3. Molecular Docking and Dynamics  
- Docking performed using PRMT5 crystal structure (**PDB ID: 8VEO**).  
- Top hits (CHEMBL4539612 & CHEMBL4577464) evaluated for binding affinity and interaction networks.  
- **250-ns MD simulations** conducted using **Desmond** to analyze RMSD, RMSF, rGyr, SASA, PSA, and MM-GBSA energies.

### 🌐 4. Network Pharmacology and Enrichment Analysis  
- A **PRMT5-centered PPI network** constructed using **STRING** (confidence ≥ 0.7).  
- Functional enrichment performed through **ChEA3**, **Enrichr**, and **KEGG** databases.  
- Visualization and clustering completed in **Cytoscape**, highlighting pathways such as histone methylation and spliceosomal assembly.

---

## 📊 Key Findings
- **CHEMBL4539612** and **CHEMBL4577464** exhibited the highest predicted activity and stable PRMT5 binding.  
- Both ligands maintained strong hydrogen bonding with catalytic residues (Asp419, Met420, Glu392, Tyr324, and Lys333).  
- MD trajectories confirmed structural equilibrium within 25–30 ns, with compact complexes and stable RMSD patterns.  
- MM-GBSA free energy analysis indicated favorable van der Waals and lipophilic stabilization.  
- Network analysis suggested that PRMT5 inhibition may modulate pathways involved in **histone methylation**, **RNA splicing**, and **gene expression control**.

---

## 🧱 Repository Structure


---

## 🧠 Technologies & Tools Used
- **Python** (scikit-learn, pandas, numpy, matplotlib, shap)  
- **PaDEL-Py** for descriptor generation  
- **Desmond / Maestro** for MD simulation  
- **AutoDock / PyMOL** for docking and visualization  
- **STRING, ChEA3, Enrichr, KEGG, Cytoscape** for network and enrichment analyses  

---

## 📈 Citation
If you use this repository, please cite:  
**Imran Mohd., et al. (2025).**  
*Structural Mechanisms and Molecular Insights into PRMT5 Inhibition.*  

---

## 📜 License
This project is licensed under the **MIT License** – you are free to use, modify, and distribute it with proper attribution.  

---

For collaborations, issues, or dataset requests, please open a GitHub issue or contact via email.  

---

⭐ **If you find this repository useful, please star it and cite our work!**
