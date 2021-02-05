# CompMedicineProject
Project repository for 02-518 project: designing a neoantigen immunogenicity prediction algorithm to predict binding affinities and immunogenicities of mutant protein-Human Leukocyte Antigen (HLA) peptide pairs  


# Contents
bibliography: contains the research papers that inspired our method designs.

input: contains the input training and benchmark datasets for our methods.
- binding_train_pseudo.csv contains pseudosequence encodings of HLA peptide sequences, each pseudosequence paired with an IC50 binding score.

- db_pepNeo_high.xls contains pseudosequence encodings of HLA peptide sequences that demonstrate high-strength binding affinity.

- db_pepNeo_medium.xls contains pseudosequence encodings of HLA peptide sequences that demonstrate medium-strength binding affinity. 

- immunogenicity_train_pseudo contains pseudosequence encodings of HLA peptide sequences, each pseudosequence paired with an immunogenicity score of 0 or 1. An immunogenicity score of 1 indicates that the sequence induces an immune response; a score of 0 indicates the sequence is not immunogenic.

metrics-outputs: contains various metrics for evaluating the performance of our methods. AUC (Area Under the Curve) scores, F1 scores, and PPV (positive predictive value) were analyzed and compared over all methods.

02518-project-bilstm-attention.ipynb is a jupyter notebook of our recurrent neural network model of a Bidirectional Long-Short Term Memory (BiLSTM). 

02518-project-convolutional.ipynb is a jupyter notebook of our convolutional neural network models. We present code for models based on residual neural networks (ResNet) and VGG neural networks.

02518-project-mlp.ipynb is a jupyter notebook of our Multilayer Perceptron (MLP) model for predicting binding/immunogenicity.

02518-project-metrics.ipynb is a jupyter notebook of our metrics calculation code.
