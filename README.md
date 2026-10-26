# Breast Cancer Tree Explorer

A planned research and educational project exploring how decision-tree
complexity affects breast-mass classification, with an interactive view
of the rules behind individual predictions.

## Current status

Research design and implementation planning.

The dataset has been downloaded and its documentation reviewed.
Model training, evaluation and the interactive prediction explorer
are not yet completed. No experimental results are reported.

## Research question

How does decision-tree depth affect classification performance
and model complexity on the Wisconsin Diagnostic Breast Cancer dataset?

## Dataset

We will use the Wisconsin Diagnostic Breast Cancer (WDBC) dataset
from the UCI Machine Learning Repository.

- 569 observations.
- 30 numerical measurements derived from images of cell nuclei
  in fine-needle aspirate samples.
- Recorded diagnosis: benign or malignant.
- The ID and diagnosis will not be included in model inputs.

Dataset:
https://archive.ics.uci.edu/dataset/17/breast-cancer-wisconsin-diagnostic

## Planned analysis

1. Load and check the dataset.
2. Reserve a stratified 20% test set.
3. Compare decision trees with maximum depths of 2, 3, 4 and 5.
4. Include one Random Forest as a more complex reference.
5. Use cross-validation within development data for model selection.
6. Evaluate the agreed models on the same held-out test observations.

We will report accuracy, balanced accuracy, sensitivity, specificity
and error counts alongside tree depth, leaf count, features used
and decision-path length.

## Planned web application

The application will allow visitors to:

- Select a test observation.
- View its predicted class.
- Follow the exact measurement-based rules used by a decision tree.
- Compare the prediction with the recorded diagnosis.
- Compare model performance and inspect mistakes.

A tree's explanation will describe that tree's own prediction.
It will not be presented as an explanation of the Random Forest.

## Next milestone

Create a reproducible notebook that loads and checks the data,
then train the first small decision tree.

## Limitations

This is a small benchmark study using established methods.
No new algorithm, clinical benefit or improved user trust is claimed.

The models will explain their decision paths, not the biological
causes of cancer. No external or prospective validation is planned.

Research and educational use only.
Not for patient diagnosis or treatment decisions.
