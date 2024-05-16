## AFFIPred: AF2 Structure-based Functional Impact Predictor
### Overview

This repository contains the Jupyter notebooks of a novel XGBoost-based pathogenicity classifier, AFFIPred, showcasing the implementation and assessment results for classification of the functional impact of missense variations. Hyperopt package was used for hyperparameter tuning with 200 evaluations. Three AFFIPred models were trained employing a nested cross-validation strategy with an outer loop of 10 folds and inner loop of 5 folds. AFFIPred represents a novel approach in pathogenicity classification by integrating both sequence and AF2-based structural information, overcoming the inherent limitations of conventional structure-based classifiers while preserving high accuracy.

ROC AUC-based performance comparison of AFFIPred against 40 other scores is depicted in the figure below, reflecting the comparable level of AFFIPred!s performance and superior coverage. The analysis was conducted on an unseen test set that does not contain any proteins present in AFFIPred's training data, ensuring the robustness of the evaluation.
 
![auc_coverage](https://github.com/timucinlab/AFFIPred/assets/58934249/ace462e6-1af4-4800-9ec6-2105384f26bc)

### Usage

Visit for the predictions of all possible variations in the human proteome:

https://affipred.timucinlab.com/

#### AFFIPred command line tool:

For installation:

```pip install affipred```

Provide input and output files:

```affipred variants.vcf -o affipred_results.csv```

For more details: https://github.com/mustafapir/AFFIPred-cli

### Citation

Pir, Mustafa Samet, & Timucin, Emel. (2024). AFFIPred: AlphaFold2 Structure-based Functional Impact Prediction of Missense Variations. bioRxiv, 2024.2005.2013.593840. doi: 10.1101/2024.05.13.593840

```bibtex
@article {Pir2024.05.13.593840,
	author = {Pir, Mustafa Samet and Timucin, Emel},
	title = {AFFIPred: AlphaFold2 Structure-based Functional Impact Prediction of Missense Variations},
	elocation-id = {2024.05.13.593840},
	year = {2024},
	doi = {10.1101/2024.05.13.593840},
	publisher = {Cold Spring Harbor Laboratory},
	URL = {https://www.biorxiv.org/content/early/2024/05/15/2024.05.13.593840},
	eprint = {https://www.biorxiv.org/content/early/2024/05/15/2024.05.13.593840.full.pdf},
	journal = {bioRxiv}
}
```
### License

This project is licensed under the MIT License.
