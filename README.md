# L2DHF: Learning to defer with human feedback
## Article 
Adaptive alert prioritisation in security operations centres via learning to defer with human feedback

## Description
Effective alert prioritisation (AP) is crucial in security operations centres (SOCs) to help analysts identify and properly respond to critical alerts amid the overwhelming volume of daily alerts, thereby improving the organisation security and minimising alert fatigue. A promising solution to AP is human-AI teaming (HAT), which combines human expertise with AI’s computational capabilities. We propose **Learning to defer with human feedback (L2DHF)**, an adaptive and real-time HAT framework for AP in SOCs. L2DHF effectively improves AP accuracy and reduces analyst workload, resulting in improved threat detection and reduced analyst fatigue. 

This repository contains the source codes and processed datasets for the implementation of L2DHF and experiments presented in the article.

## Datasets
Two publicly available datasets, UNSW-NB15 and CICIDS2017, are used to run the experiments and evaluate the L2DHF framework. The original datasets are available in the following links:

UNSW-NB15: https://research.unsw.edu.au/projects/unsw-nb15-dataset

CICIDS2017: https://www.unb.ca/cic/datasets/ids-2017.html 

The pre-processed datasets used in experiments are available in the folders, named: DatasetUsedinExperiments_[name of dataset].

## Experiments
The folder of Experiments_[name of dataset] contains the source codes of L2DHF, baseline and state-of-the-art (SOTA) models. 

## Classifiers of Ensemble
These are the files of fine-tuned, optimised, and trained classifiers, which are used in experiments to build the Predictive AI and A2C models. They are placed in ClassifiersOfEnsemble_[name of dataset] folder for experiments related to each dataset.

## Performance Evaluation
The PerformanceEvaluation_[name of dataset] folder provides the source codes for generating the performance values and graphs related to the used dataset in the article. 

## Isolation Forest for AlertPro
The folder of IsolationForest_for_AlertPro_[name of dataset] provides the trained isolation forest model related to the used dataset to run AlertPro as a SOTA model. 

## Instructions to Run Experiments
- Put classifier files or the isolation forest file in the same folder of the related experiment file (e.g., L2DHF_CICIDS2017.ipynb) to run that experiment.
- Make sure the version of python and libraries are the same as indicated in the beginning of the experiment notebook file.
- Make sure the file path of the datasets in the code is correct.
- Create a folder to save the .json files as the results of experiments and make sure its file path (in front of: **output_folder**) is correct.
- Run the cells of the notebook file sequentially.

## Code Developer
**Name:** Fatemeh Jalalvand

**Email:** fateme.jalalvand@gmail.com 

## Citation
If you use the codes or data in your work, please cite the following paper:

Jalalvand, F., Chhetri, M. B., Nepal, S., & Paris, C. (2025). Adaptive alert prioritisation in security operations centres via learning to defer with human feedback. arXiv preprint arXiv:2506.18462, .

BibTeX format:

@article{jalalvand2025adaptive,

title = {Adaptive alert prioritisation in security operations centres via learning to defer with human feedback},

author = {Jalalvand, Fatemeh and Chhetri, Mohan Baruwal and Nepal, Surya and Paris, C{\\'e}cile},

journal = {arXiv preprint arXiv:2506.18462},

year = {2025}

}

## Acknowledgments
This work was supported by CSIRO’s Collaborative Intelligence (CINTEL) Future Science Platform (FSP).

Also, this project was supported by resources provided by CSIRO IMT Scientific Computing.
