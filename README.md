# **Physical Activity and Type 2 Diabetes Mellitus**
Data from the World Health Organization shows that the number of people with type 2 diabetes mellitus (T2DM) skyrocketed from 108 million in 1980 to 422 million in 2014. Not surprinsingly considering our current lifestyle, the prevalence has been sharply rising: there was a **3%** increase in diabetes **mortality rates** by age between 2000 and 2019. Diabetes is a major cause of blindness, kidney failure, heart attacks, stroke, and lower limb amputation. Thus, it is considered one of the greatest public health concerns of the 21th century.  

**Physical activity** has been demonstrated as a critical part of the treatment of this chronic condition. However, there is no consistent evidence about which and how much physical activity these people should engage to improve their global health. Therefore, this repository tries to clarify this information, providing the required data to reproduce the results presented in the scientific works that arose from this research question. We firstly focused on one of the most interesting outcomes in diabetes: the **glycosylated hemoglobin** (HbA1c). Next, we explored the effectiveness of physical activity in a health condition that is strongly associated with T2DM: **hypertension**.

## Glycosylated hemoglobin
In this repository you will find the `Glycosylated Hemoglobin (HbA1c)` folder that contains all the documentation needed to reproduce the results of the manuscript entitled **Optimal Dose and Type of Physical Activity to Improve Glycemic Control in People Diagnosed With Type 2 Diabetes: A Systematic Review and Meta-Analysis** published in Diabetes Care (link: https://diabetesjournals.org/care/article/47/2/295/154149/Optimal-Dose-and-Type-of-Physical-Activity-to).  

For a better understanding of the dataset that you have to import in R (read the intructions below), we state a short description of the variables you will find within the dataset. 

### Download the Excel file
First, the dataset in Excel format must be downloaded. It has all the required data to conduct the posterior analyses presented in the R code file. For a better understanding of the data, here we explain the variables meaning.

### Variables' explanation
  + `studyID` is the included studies in this meta-analysis. Each row (i.e., observation) corresponds to each study-arm.
  + `N` is the total sample of the study.
  + `age` is the average age of each study.
  + `sex_male` is the number of males within the study sample.
  + `supervised` corresponds to whether or not the intervention was supervised by a physical activity/ fitness/ medical/ physiotherapy professional.
  + `baseline_glyc` (if reported) is the average baseline level of glycemia that participants begin the intervention.
  + `ìllness_duration` is the duration between the diagnosis of diabetes and the intervention beginning.
  + `BMI` is the average body mass index (BMI) of the study sample.
  + `agent` is the type of physical activity performed on each study.
  + `outcome` corresponds to our outcome of interest.
  + `pren` is the study sample at baseline.
  + `premean` is the mean value of glycemia level at baseline.
  + `presd` is the standard deviation of the mean glycemia value at baseline.
  + `postn` is the study sample at post-intervention time point.
  + `postmean` is the mean value of glycemia level at post-intervention time point.
  + `postsd` is the standard deviation of the mean glycemia value at post-intervention time point.
  + `y` represents the mean change from baseline within the study arm.
  + `se` is the standard error of the mean change from baseline.
  + `diff` is the mean difference between study-arms at post-intervention time point.
  + `pooled_var` ia the pooled variance within a study.
  + `se_diff` corresponds to the standard error of the mean difference (when `diff` = `NA`, then the standard error of the mean change and the mean difference were identical).
  + `outcome_group` is the outcome of interest.
  + `lower_is_better`corresponds to the direction of the outcome: the lower the value, the greater the improvement.
  + `Notes`is the variable where we specify the intervention parameters.
  + `trt` is the most specific level showing what studies had performed.
  + `duration_weeks` is the duration in weeks of the interventions.
  + `sessions` represents the frequency of the intervention (i.e., number of sessions per week).
  + `time_session` is the minutes an intervention session lasted.
  + `code_compendium` is the code that belongs the classification made by the international and validated *Compendium of Physical Activities*.
  + `dose_calculation` corresponds to the METs-min/day (i.e., daily dose of physical activity) of each study-arm.
  + `weekly_dose` is the daily dose multiplied by the intervention frequency, obtaining the weekly dose of physical activity (i.e., mETs-min/week).
  + `dose_by_50` is the approximation of weekly dose by 50 METs-min/week increments (that is to favour the data exploratory analysis).
  + `dose_by_100` is the approximation of weekly dose by 100 METs-min/week increments.

#### File path inspection
Friendly reminder: you have to fill the gap of the file path within the code when the dataset is imported in our R environment.


## Hypertension
Additionally, you will also find in this repository the `Hypertension` folder, which contains the documentation needed to reproduce the analyses conducted in *title of the manuscript that is not finished yet*. To ease the data import, we export directly the clean dataset from our R environment, and save it in a `.Rda` doc, which can be directly read in R. So, you just have to download the `SBP_data` and `DBP_data` from the aforementioned repository, and run the code in your console.

