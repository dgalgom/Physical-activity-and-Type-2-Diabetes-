# Physical-activity-and-Type-2-Diabetes-
This is the repository where we state all the information to reproduce the results of our manuscript entitled "Optimal Dose and Type of Physical Activity to Improve Glycemic Control in People Diagnosed With Type 2 Diabetes: A Systematic Review and Meta-Analysis" published in Diabetes Care.

## Download the Excel file
First, the dataset in Excel format must be downloaded. It has all the required data to conduct the posterior analyses presented in the R code file. For a better understanding of the data, here we explain the variables meaning.

## Variable explanation
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

### File path inspection
Friendly reminder: you have to fill the gap of the file path within the code when the dataset is imported in our R environment.
