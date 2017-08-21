# PVP-modifications

### Pre-requisite:
* Python
* CUDA
* CUDNN5.1
* Jupyter Notebook
* Tensorflow and keras
* Nvidia GPU
   
### Data:
Data can be downloaded from this [link](https://drive.google.com/open?id=0B-hYmS2zP3aZM2I1akVZV2RKMnc)

### File Descriptions:
* Final Experiments: Code to create 8 DNN models. Models are not saved.
     Run the first block and skip the "Dataset" section. 
     
     To get the model train the DNN with appropriate train sets. Different train sets will give different models.
     
     Directly go to **Model** section. Change the training dataset and **dimension of X**.
     In Model Name Save the name of the particular model (eg. filepath="MODEL1.weights.best.hdf5").
     
     Go to "Test" section, update the Model weights same as Training Model, and run tests.
     Then use the same Test Model to test the 1000 files on a loop & get the scores. 
     (File Format should be same as train/test sets)
     
     Then Go to CELL DATA section. Train the model with cell data & test it with the above procedure.
     
     In ***DNN Tissue Model 1***, Scores and Test File sector, there is function for generating 1000 scores. (You also have to take care      of missing values by average and set a flag)
     
 * Stats Fun: Some Stastical analysis of the data.

### Data Description:
* PVP_feature_train/test : Normal PVP features dataset.
* PVP_features_no_braca_test/train : Normal PVP features without BRCA.
    > Train PVP_features and test bot PVP_test and PVP_test_no_brca and vice versa(2 models, 4 tests)

* tissue_brca_train/test: Normal PVP with human tissues.
* tissue_no_brca_test/train: Normal PVP with no BRCA genes
   > (2 models, 4 tests)
   
* norm_tissue_brca_test/train: Row Normalised tissues with PVP features.
* norm_tissue_no_brca_test/train: Row Normalised tissues with PVP features with no BRCA genes.
   > (2 models, 4 tests)

### Documentation will be updated properly soon!
    I have just written how to train and test the models. This is not general purpose documentation.
    I am facing some problem installing CUDA and running the notebooks on my PC. I will try to do it as soon as this is fixed.
    Please email me if facing any problem during runs.
