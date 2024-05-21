## Data and code associated with the manuscript "An atlas of plasma extracellular vesicle proteins distinguishing cancer and doxorubicin sensitivity"

This reposotory includes the code and key summary tables related to the manuscript by Van Tine _et al._ focused on sarcoma extracellular vesicles. Several of the steps are best performed on a computer cluster to ensure sufficient memory.

All proteomic data for the Sarcoma cohort is deposited in UCSD’s [Massive](massive.ucsd.edu) with ID MSV000092188. Reviewers can use the username MSV000092188_reviewer and password VanTine_001_0616 to anonymously access the data. The FTP download link is ftp://MSV000092188@massive.ucsd.edu. Accessing data for the Hoshino _et al._ dataset is detailed in their [Cell manuscript](https://www.sciencedirect.com/science/article/pii/S0092867420308746?via%3Dihub).

### File details
* SampleMetadata.xlsx: Sample metadata for Sarcoma cohort
* expt_smty.xlsx: Annotation file needed for ProteoQ processing of Sarcoma cohort
* ProteinQuantitationWithSampleMetadata.xlsx: Final protein-level quantitation of the Sarcoma cohort with sample metadata added
* uniprotAnnotationsForFigure2.xlxs: Uniprot annotations for Figure 2
* dfHarmonizer.txt: used to harmonize sarcoma and Hoshino datasets
* dfMerged_description.csv: used to harmonize sarcoma and Hoshino datasets
* _selectedFeaturesRFECV_target-dfHarmonizedCancer_nSampleFilter60_trainFrac-0.75_wholeDataset.json: selected features for KNN pan-cancer classification
* studyKNeighborsClassifier_dfHarmonizedCancer_nSampleFilter60_trainFrac-0.75_wholeDataset.db: KNN pan-cancer classifier as a db file
* KNeighborsClassifierTuned_target-dfHarmonizedCancer_nSampleFilter60_trainFrac-0.75_wholeDataset.pkl: KNN pan-cancer classifier as a pkl file

### Jupyter notebook details
* for all notebooks use Python v3.10, R v 4.2.1, jupyterlab v 4.1.1, pandas v2.0.0, numpy v1.23.4, scikit-learn v1.3.2, joblib v1.3.2, statsmodels v 0.14.0, scipy v 1.10.1, pingoin 0.5.3, openpyxl v 3.0.10, optuna v3.5.0, xgboost v2.0.3, catboost v1.2.3, lightgbm v4.3.0, rpy2 v3.5.9, and pip 24.0.
* Notebook VanTineEtAl_ProteoQ.ipynb is used for ProteoQ processing of the Sarcoma cohort and to generate some panels of Figure 2.
* Notebook VanTineEtAl_Fig1_LinePlot.ipynb is used to generate the line plot in Figure 1.
* Notebook VanTineEtAl_Fig2_VolcanoPlot.ipynb is used to generate the volcano plot (sarcoma vs. healthy) in Figure 2.
* Notebook VanTineEtAl_Fig2_Catplot.ipynb is used to generate the catplot in Figure 2.
* Notebook VanTineEtAl_Fig3_panCancerClassification.ipynb is used for the pan-cancer classification in Figure 3.
* Notebook VanTineEtAl_Figs3&4_AllButClassification.ipynb is used for the non-classification plots in Figures 3 & 4.
* Notebook VanTineEtAl_Harmonizer.ipynb is used to harmonize the sarcoma and Hoshino datasets. Uses R v4.2.1.
* Notebook VanTineEtAl_Fig5_VolcanoPlot_resistantPatients_PreVsPost.ipynb.ipynb is used to generate the volcano plot (pre vs. post treatment in drug resistant sarcoma patients) in Figure 5.
* Notebook VanTineEtAl_Fig5_VolcanoPlot_sensitivePatients_PreVsPost.ipynb.ipynb is used to generate the volcano plot (pre vs. post treatment in drug sensitive sarcoma patients) in Figure 5.
* Notebook VanTineEtAl_Fig5_VolcanoPlot_SvR.ipynb is used to generate the sensitive:resistant volcano plot in Fig 5.
* Notebook VanTineEtAl_Fig5_LDA.ipynb is used to generate the LDA-related plots in Figure 5.
* Notebook VanTineEtAl_Fig5_Classification.ipynb is used for the sarcoma vs healthy and doxorubicin sensitivity classification in Figure 5.
* Notebook VanTineEtAl_Fig5_Catplot.ipynb is used to generate the catplots in Figure 5.
* Note to self: don't forget the notebook to make dfHarmonized
