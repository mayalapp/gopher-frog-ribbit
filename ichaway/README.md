# FLSHE folder README

## Summary

This folder is to help researchers/land managers process data using the gopher frog RIBBIT model at Fall Line Sandhills East. 

## Files/folders

* `1-run_model_to_get_ribbit_scores.ipynb` - use this file to run the gopher frog model on new data and export a csv file with the RIBBIT scores 
* `2-organize_ribbit_data.ipynb` - use this to: 
   1. Combine multiple csv files with RIBBIT scores
   2. Extract the top RIBBIT scores to a new csv file
* `3-combine-ribbit-scores-with-verified-data.ipynb` - use this to create a csv file with both RIBBIT scores and manually verified data (0 for no gopher frog 1 for yes gopher frog). This csv file can be used to evaluate how well the model is doing. 

* `sample_data` - a folder with sample data (this data is fake!) of how data should be organized to run `1-run_model_to_get_ribbit_scores.ipynb` 
* `results_Dec2022` - Model results as of December 2022
   1. `param_values.txt` - file containing parameter values used for model
   2. `ribbit_scores_combined.csv` - all ribbit scores outputted by model
   3. `ribbit_scores_with_verified_data.csv` - verified data combined with ribbit scores - can be used to evaluate model 
* `verified_flshe` - Folder with a csv file of manually verified data. Add to this file as we listen to more data. 

## Run model on other data

Use `1-run_model_to_get_ribbit_scores.ipynb` to run the model on your data. Your data must follow the structure in `sample_data`, but you can change the folder path to a different folder (including an external drive). 

## Current issues

* Need to be able to group files by wetland
* Some of the file names in the verified Ichaway data have different values for the "minutes" than the actual audio files. This means when merging the verified data with the RIBBIT scores, we either (A) lose some data or we (B) assume the minutes indicator is unimportant. Currently we are using option (A), as it is more reliable, but we do lose some of our data. 


  
  