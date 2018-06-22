# MedicalData
This is a comprehensive Exploratory Data Analysis for the [Personalized Medicine: Redefining Cancer Treatment](https://www.kaggle.com/c/msk-redefining-cancer-treatment) challenge. 

Using *ggplot2* and the *tidyverse* tools to study and visualise the structures in the data.  Challenge to automatically classify genetic mutations that contribute to cancer tumor growth (so-called "drivers") in the presence of mutations that don't affect the tumors ("passengers").  


The [data](https://www.kaggle.com/c/msk-redefining-cancer-treatment/data) comes in 4 different files.
Two csv files and two text files:  


- *training/test variants:* These are csv catalogues of the gene mutations together with the target value *Class*, which is the (manually) classified assessment of the mutation. The feature variables are *Gene*, the specific gene where the mutation took place, and *Variation*, the nature of the mutation. 

The test data of course doesn't have the *Class* values. This is what we have to predict. These two files each are linked through an *ID* variable to another file each, namely: 

- *training/test text:* Those contain an extensive description of the evidence that was used (by experts) to manually label the mutation classes.  The text information holds the key to the classification problem and will have to be understood/modelled well to achieve a useful accuracy.
