Contact
SHahan Syed
PhD researcher, University of Helsinki
Phone:      +358 405 524595
LinkedIn:  www.linkedin.com/in/syed-shahan
E-mail:    shahan.syed@helsinki.fi
ORCID:     0000-0001-9861-6441


•	Data Preparation:
o	Data split into four references using Pandas library in Jupyter notebooks:
	Control: before vs after venticulator
	Disease: before and after venticulator
o	Proteins missing in more than 30% of samples were removed.
o	Exploratory Data Analysis (EDA) performed for initial insights.
•	Variance Stabilization and Normalization:
o	High variance identified in some samples.
o	Used Bioconductor in R for variance stabilization normalizatio (VSN)
o	Implemented in Python using R2Py.
o	Stabilization applied with proteins in rows and samples in columns.
•	Summary Statistics:
o	Checked for variance, mean, standard deviation, etc. (please see file attached)
•	Random Forest Imputation:
o	Imputation performed for missing values using Random Forest separately for all 4 dataframes.
o	Fine-tuned parameters:
	finetuned model parameters with RMSE
	Parameters tested:
	Number of estimators (5, 10, 15)
	Iterations (5, 10, 15)
	Randomness (42(default), 25, 50)
•	Data Analysis:
o	Random Forest Imputation applied to each dataframe sepertely 
o	Data compiled for analysis.
o	student T-tests conducted (Equal Sample Size Normalization already applied).
o	False Discovery Rate (FDR) correction applied (Benjemini Hochberg method from scikitlearn)
Improvements:
•	Normalization step was added. VSN was applied.
•	Quality of RF imputation was checked and parameters were finetuned based on RMSE of the predicted vs original values
•	Yaml file was added to manage and integrate the workflow better

