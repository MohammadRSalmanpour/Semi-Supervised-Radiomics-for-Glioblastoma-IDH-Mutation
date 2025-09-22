# Semi-Supervised-Radiomics-for-Glioblastoma-IDH-Mutation

**Title:** Semi-Supervised Radiomics for Glioblastoma IDH Mutation: Limited Labels, Data Sensitivity, and SHAP Interpretation  

---

## 📖 Overview
This repository contains the code, supplemental files, and results for our paper:  

*Semi-Supervised Radiomics for Glioblastoma IDH Mutation: Limited Labels, Data Sensitivity, and SHAP Interpretation.*  

Glioblastoma (GBM) is one of the most aggressive brain tumors. **IDH mutation status** is a crucial prognostic biomarker, but conventional testing requires invasive biopsies.  
This work introduces a **semi-supervised learning (SSL) framework** that leverages **multi-sequence MRI radiomics** (T1, T2, T1CE, FLAIR) to predict IDH status.  

We systematically compared **supervised (SL)** and **semi-supervised (SSL)** models across **8 multicenter datasets** (n = 1,329 patients) and incorporated **SHAP-based interpretation** for feature importance analysis.  

---

## 🧪 Key Contributions
- ✅ First large-scale multicenter SSL framework for IDH prediction  
- ✅ Integration of **38 feature selection/attribute extraction methods** and **24 classifiers**  
- ✅ Comprehensive **cross-validation and external validation** (UCSF-PDGM, UPENN-GBM, IvyGAP, TCGA-GBM, TCGA-LGG)  
- ✅ Data sensitivity analysis under varying labeled/unlabeled proportions  
- ✅ SHAP interpretability to identify **stable and biologically relevant radiomic biomarkers**  

---

## 📊 Main Results

**Best SSL model (RFE + SVM):**
- Cross-validation accuracy: **0.93 ± 0.01**  
- External accuracy: **0.75 ± 0.02**  
- High F1 (0.94 CV, 0.74 test) and AUC (0.97 CV, 0.84 test)  

**Best SL model (RFE + Complement Naïve Bayes):**
- Cross-validation accuracy: **0.90 ± 0.02**  
- External accuracy: **0.80 ± 0.006**  

**Key findings:**
- Multimodal MRI (**T1+T2+T1CE+FLAIR**) consistently outperformed single-sequence models  
- SSL reduced sensitivity to dataset size, enabling robust performance with limited labels  
- SHAP analysis highlighted the importance of **FO_RMS (T1CE)** and **wavelet-derived features**  

---

## 📑 Citation
If you use this repository in your work, please cite:  

Pouria, A.H., Jabarzadeh Ghandilu, S., Taeb, S., Mehrnia, S.S., Oveisi, M., Hacihaliloglu, I., Rahmim, A., Salmanpour, M.R.  
*Semi-Supervised Radiomics for Glioblastoma IDH Mutation: Limited Labels, Data Sensitivity, and SHAP Interpretation.* 2025.  

---

## 🙏 Acknowledgements
This project was supported by:  
- **Virtual Collaboration Group (VirCollab)** and **TECVICO CORP.**  
- **Canadian Foundation for Innovation – John R. Evans Leaders Fund (CFI-JELF)**  
- **NSERC Discovery Grants**  
