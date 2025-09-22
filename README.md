# Semi-Supervised-Radiomics-for-Glioblastoma-IDH-Mutation

**Title:** Semi-Supervised Radiomics for Glioblastoma IDH Mutation: Limited Labels, Data Sensitivity, and SHAP Interpretation  


## 📖 Overview
This repository contains the code, supplemental files, and results for our paper:  

*Semi-Supervised Radiomics for Glioblastoma IDH Mutation: Limited Labels, Data Sensitivity, and SHAP Interpretation.*  

Glioblastoma (GBM) is one of the most aggressive brain tumors. **IDH mutation status** is a crucial prognostic biomarker, but conventional testing requires invasive biopsies.  
This work introduces a **semi-supervised learning (SSL) framework** that leverages **multi-sequence MRI radiomics** (T1, T2, T1CE, FLAIR) to predict IDH status.  

We systematically compared **supervised (SL)** and **semi-supervised (SSL)** models across **8 multicenter datasets** (n = 1,329 patients) and incorporated **SHAP-based interpretation** for feature importance analysis.  


## 🧪 Key Contributions
- ✅ First large-scale multicenter SSL framework for IDH prediction  
- ✅ Integration of **38 feature selection/attribute extraction methods** and **24 classifiers**  
- ✅ Comprehensive **cross-validation and external validation** (UCSF-PDGM, UPENN-GBM, IvyGAP, TCGA-GBM, TCGA-LGG)  
- ✅ Data sensitivity analysis under varying labeled/unlabeled proportions  
- ✅ SHAP interpretability to identify **stable and biologically relevant radiomic biomarkers**  


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


## 📂 Repository Structure
Supplemental File 1 contains the machine learning performance results for Supervised Learning (SL) using FLAIR. Sheet 1 (“Selected_Features”) represents the top 10 features selected by each feature selector or attribute extraction method. Sheet 2 (“Best_Parameters”) represents the optimal hyperparameters of the applied machine learning algorithms. Sheet 3 (“Aggregated_Results”) represents the aggregated validation and test performance metrics, including Accuracy, Precision, AUC, F1-score, Recall, and Specificity. Sheet 4 (“Aggregated_Std_Results”) represents the corresponding standard deviation values. Supplemental File 2 contains the machine learning performance results for SL using Combined sequences. (Sheets 1–4 as described above). Supplemental File 3 contains the machine learning performance results for SL using T1. (Sheets 1–4 as described above). Supplemental File 4 contains the machine learning performance results for SL using T1CE. (Sheets 1–4 as described above). Supplemental File 5 contains the machine learning performance results for SL using T2. (Sheets 1–4 as described above). Supplemental File 6 contains the machine learning performance results for Semi-Supervised Learning (SSL) using FLAIR. (Sheets 1–4 as described above). Supplemental File 7 contains the machine learning performance results for SSL using Combined sequences. (Sheets 1–4 as described above). Supplemental File 8 contains the machine learning performance results for SSL using T1. (Sheets 1–4 as described above). Supplemental File 9 contains the machine learning performance results for SSL using T1CE. (Sheets 1–4 as described above). Supplemental File 10 contains the machine learning performance results for SSL using T2. (Sheets 1–4 as described above).


## 📑 Citation
If you use this repository in your work, please cite:  

Pouria, A.H., Jabarzadeh Ghandilu, S., Taeb, S., Mehrnia, S.S., Oveisi, M., Hacihaliloglu, I., Rahmim, A., Salmanpour, M.R.  
*Semi-Supervised Radiomics for Glioblastoma IDH Mutation: Limited Labels, Data Sensitivity, and SHAP Interpretation.* 2025.  

## 🙏 Acknowledgements
This project was supported by:  
- **Virtual Collaboration Group (VirCollab)** and **TECVICO CORP.**  
- **Canadian Foundation for Innovation – John R. Evans Leaders Fund (CFI-JELF)**  
- **NSERC Discovery Grants**  
