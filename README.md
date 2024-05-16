## AFFIPred: AF2 Structure-based Functional Impact Predictor

A novel structure-based pathogenicity classifier, AFFIPred, merges both sequence and AF2-based structural information. This combination tackles limitations of traditional structure-based classifiers while maintaining accuracy. 
This repository contains jupyter-notebook files for training of three AFFIPred models and performance assessment results. 

Visit for the predictions of all possible variations in the human proteome:

https://affipred.timucinlab.com/

For installation:

```pip install affipred```

Provide input and output files:

```affipred variants.vcf -o affipred_results.csv```


![auc_coverage](https://github.com/timucinlab/AFFIPred/assets/58934249/ace462e6-1af4-4800-9ec6-2105384f26bc)
