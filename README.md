# post_error_followup

## directory structure
    ├── build
    │   └── temp.linux-x86_64-3.10
    │       └── home
    │           └── adkinsty
    ├── inference.ipynb
    ├── input
    │   ├── model_inputs
    │   │   ├── model_inputs_memory2.json
    │   │   ├── model_inputs_memory_color_long.json
    │   │   ├── model_inputs_memory_color_short.json
    │   │   └── model_inputs_memory.json
    │   ├── preprocessors
    │   │   ├── subj_encoder_memory2.pkl
    │   │   ├── subj_encoder_memory_color_long.pkl
    │   │   ├── subj_encoder_memory_color_short.pkl
    │   │   └── subj_encoder_memory.pkl
    │   └── raw_data
    │       ├── raw_data_memory2.csv
    │       ├── raw_data_memory_color_long.csv
    │       ├── raw_data_memory_color_short.csv
    │       └── raw_data_memory.csv
    ├── output
    │   ├── group_par
    │   │   ├── dat
    │   │   │   ├── group_par_invar_beta_memory2.csv
    │   │   │   ├── group_par_invar_beta_memory_color_long.csv
    │   │   │   ├── group_par_invar_beta_memory_color_short.csv
    │   │   │   ├── group_par_invar_beta_memory.csv
    │   │   │   ├── group_par_var_beta_memory2.csv
    │   │   │   ├── group_par_var_beta_memory_color_long.csv
    │   │   │   ├── group_par_var_beta_memory_color_short.csv
    │   │   │   └── group_par_var_beta_memory.csv
    │   │   └── fig
    │   │       ├── beta_diff_invar_beta_memory2.png
    │   │       ├── beta_diff_invar_beta_memory_color_long.png
    │   │       ├── beta_diff_invar_beta_memory_color_short.png
    │   │       ├── beta_diff_invar_beta_memory.png
    │   │       ├── beta_diff_var_beta_memory2.png
    │   │       ├── beta_diff_var_beta_memory_color_long.png
    │   │       ├── beta_diff_var_beta_memory_color_short.png
    │   │       ├── beta_diff_var_beta_memory.png
    │   │       ├── mu_diff_invar_beta_memory2.png
    │   │       ├── mu_diff_invar_beta_memory_color_long.png
    │   │       ├── mu_diff_invar_beta_memory_color_short.png
    │   │       ├── mu_diff_invar_beta_memory.png
    │   │       ├── mu_diff_var_beta_memory2.png
    │   │       ├── mu_diff_var_beta_memory_color_long.png
    │   │       ├── mu_diff_var_beta_memory_color_short.png
    │   │       ├── mu_diff_var_beta_memory.png
    │   │       ├── sigma_diff_invar_beta_memory2.png
    │   │       ├── sigma_diff_invar_beta_memory_color_long.png
    │   │       ├── sigma_diff_invar_beta_memory_color_short.png
    │   │       ├── sigma_diff_invar_beta_memory.png
    │   │       ├── sigma_diff_var_beta_memory2.png
    │   │       ├── sigma_diff_var_beta_memory_color_long.png
    │   │       ├── sigma_diff_var_beta_memory_color_short.png
    │   │       └── sigma_diff_var_beta_memory.png
    │   ├── group_pred
    │   │   ├── dat
    │   │   │   ├── ci_pred_invar_beta_memory2.csv
    │   │   │   ├── ci_pred_invar_beta_memory_color_long.csv
    │   │   │   ├── ci_pred_invar_beta_memory_color_short.csv
    │   │   │   ├── ci_pred_invar_beta_memory.csv
    │   │   │   ├── ci_pred_var_beta_memory2.csv
    │   │   │   ├── ci_pred_var_beta_memory_color_long.csv
    │   │   │   ├── ci_pred_var_beta_memory_color_short.csv
    │   │   │   ├── ci_pred_var_beta_memory.csv
    │   │   │   ├── pred_invar_beta_memory2.csv
    │   │   │   ├── pred_invar_beta_memory_color_long.csv
    │   │   │   ├── pred_invar_beta_memory_color_short.csv
    │   │   │   ├── pred_invar_beta_memory.csv
    │   │   │   ├── pred_var_beta_memory2.csv
    │   │   │   ├── pred_var_beta_memory_color_long.csv
    │   │   │   ├── pred_var_beta_memory_color_short.csv
    │   │   │   └── pred_var_beta_memory.csv
    │   │   └── fig
    │   │       ├── ci_pred_invar_beta_memory2.png
    │   │       ├── ci_pred_invar_beta_memory_color_long.png
    │   │       ├── ci_pred_invar_beta_memory_color_short.png
    │   │       ├── ci_pred_invar_beta_memory.png
    │   │       ├── ci_pred_var_beta_memory2.png
    │   │       ├── ci_pred_var_beta_memory_color_long.png
    │   │       ├── ci_pred_var_beta_memory_color_short.png
    │   │       └── ci_pred_var_beta_memory.png
    │   ├── metrics
    │   │   ├── waic_invar_beta_memory2.csv
    │   │   ├── waic_invar_beta_memory_color_long.csv
    │   │   ├── waic_invar_beta_memory_color_short.csv
    │   │   ├── waic_invar_beta_memory.csv
    │   │   ├── waic_var_beta_memory2.csv
    │   │   ├── waic_var_beta_memory_color_long.csv
    │   │   ├── waic_var_beta_memory_color_short.csv
    │   │   └── waic_var_beta_memory.csv
    │   ├── model_fit
    │   │   ├── model_fit_invar_beta_memory2.pkl
    │   │   ├── model_fit_invar_beta_memory_color_long.pkl
    │   │   ├── model_fit_invar_beta_memory_color_short.pkl
    │   │   ├── model_fit_invar_beta_memory.pkl
    │   │   ├── model_fit_var_beta_memory2.pkl
    │   │   ├── model_fit_var_beta_memory_color_long.pkl
    │   │   ├── model_fit_var_beta_memory_color_short.pkl
    │   │   └── model_fit_var_beta_memory.pkl
    │   └── model_fit.tar.gz
    ├── README.md
    ├── ref
    │   └── rpm1_hier.stan
    └── training.ipynb

### training
This notebook is used to fit the models
### inference
This notebook is used to evaluate and post-process the models
### input
#### raw_data 
data taken from dropbox, called `dat.csv` under each experiment subfolder
#### model_input 
data given as input to a stan model
#### preprocessors
subject id encoders can be used to map between prolific ids and integer ids used in the model
### output
#### model_fit 
stan code and posterior samples for fitted models (not added yet, need to compress first) 
#### group_par
tables and figures of group-level parameters of interest
#### group_pred
tables and figures of predicted behavior from group-level parameters
#### metrics
tables of goodness-of-fit metrics for each model (currently just WAIC)
### ref
This directory contains the reference stan code file from dropbox used in the training notebook above. 
### build
This directory contains auto-generated cache files used to avoid recompiling reused models
