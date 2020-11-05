# Exploration-of-brain-tissue-radiomics-on-clinical-and-quantitative-MRI-for-MS
  
Elizaveta Lavrova, Henry C. Woodruff,  Pierre Maquet, Eric Salmon, Emilie Lommers, Philippe Lambin, Christophe Phillips  
  
<b>Objectives</b>. Clinical magnetic resonance imaging (MRI) is poorly sensitive to some pathological changes related to multiple sclerosis (MS) in normal appearing white matter (NAWM) and grey matter (GM), and is not reproducible and comparable in cross-sectional studies. Quantitative MRI (qMRI) offers a closer representation of the physical properties of brain tissues while radiomics provides a quantitative description for medical images. The goal of this study is to investigate the diagnostic value of radiomic features in white matter (WM), NAWM, and GM, extracted from clinical and quantitative MRI. We aimed to develop exploratory radiomic binary classification models based on clinical MRI and qMRI data to distinguish between MS patients (MSP) and healthy control subjects (HCS) and to validate the clinical MRI models on an external open source database.  
<b>Materials and methods</b>. This retrospective explorative study involved 36 HCS and 36 MSP, recruited in CHU Liege, Belgium, with clinical T1w MRI and, uniquely, qMRI. Radiomic features were extracted from the WM, NAWM and GM regions and from all image types. Based on the training subset, recursive feature elimination was applied to create feature vectors for each image type and region of interest. Random forest, support vector machine, and logistic regression binary classification models (MSP vs HCS) were trained and validated on the testing subset. External validation was performed on T1w-based models using open source datasets with 167 HCS and 10 MSP.  
<b>Results</b>. Ranked by region of interest the best performance was achieved in the whole WM, where the model based on magnetization transfer (MT) imaging features yielded a median area under the receiver operating characteristic curve (AUC) of 1.00 (no confidence interval). Ranked by image type the best performance was achieved by the MT models, with median AUCs of 0.79 (0.71-0.89 90% CI) and 0.81(0.73-0.88) in NAWM and GM, respectively. External validation of the T1w models yielded an AUC of 0.78 (0.51-0.99) in whole WM, demonstrating a large 95% CI and also with a poor sensitivity of 0.30 (0.10-0.60).  
<b>Conclusion</b>. This exploratory study indicates that qMRI Radiomics could provide efficient diagnostic information using NAWM and GM analysis in MSP. T1w radiomics could eventually be useful for rapid check of clinical MRI for WM abnormalities once acquisition and reconstruction heterogeneities have been overcome. Further research is needed, involving more data, for better interpretation and generalization of the results.  

<b>Project structure</b>:  
* CRC, CC359, MSSEG - imaging data (not shared),  
* description - .csv files with the demographic information about the participants (age, gender),  
* features - .csv files with extracted feature values,    
* features_analysis - results of the preliminary features analysis in .csv,
* names - .txt files with names of the participants from DS1, DS2, and DS3 and names of the participants from DS1, distributed between train and test subsets,  
* features_to_model - .txt files with feature names, used in each image type/ROI model,  
* performance - performance metrics, obtained with each bootstrap step for each model (not shared because of the big size, to be generated),  
* outcomes - real/predicted outcome values for each bootstrap step for each model (not shared  because of the big size, to be generated),  
* scripts - python scripts with analysis pipeline.
