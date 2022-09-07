# post_error_followup

## directory structure

tbd

## training.ipynb
used to fit the models
## inference.ipynb
used to evaluate and post-process the models
## input
### raw_data 
data taken from dropbox, called `dat.csv` under each experiment subfolder
### model_input 
data given as input to a stan model
### preprocessors
subject id encoders can be used to map between prolific ids and integer ids used in the model
## output
### model_fit 
stan code and posterior samples for fitted models (not added yet, need to compress first) 
### group_par
tables and figures of group-level parameters of interest
### group_pred
tables and figures of predicted behavior from group-level parameters
### metrics
tables of goodness-of-fit metrics for each model (currently just WAIC)
## ref
reference stan code file from dropbox used in the training notebook above. 
