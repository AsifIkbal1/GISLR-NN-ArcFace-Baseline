# GISLR-NN-ArcFace-Baseline
GISLR: NN + ArcFace Baseline
GISLR: NN + ArcFace Baseline


I used the code of [GISLR: PyTorch->TFLite Baseline](https://www.kaggle.com/code/myso1987/gislr-pytorch-tflite-baseline/notebook) as a baseline.
If you want to add Arcface layer just change `CFG.arcface = True`.

## Version1
* Added  ArcFace loss with the cross entropy loss
* Train_test_split for validation
* `CV:0.6458`  , `LB:0.45`

## Version2
* No Arcface
* Train_test_split for validation
* `CV:0.6119`  , `LB:0.39`

## Version3
* Added  ArcFace loss with the cross entropy loss
* StratifiedGroupKFold for validation
* `epochs=350`
* `CV:0.39`  , `LB:0.42`

## Version4
* Added  ArcFace loss with the cross entropy loss
* StratifiedGroupKFold for validation
* Great feature generation using PyTorch model based on this [notebook](https://www.kaggle.com/code/mayukh18/end-to-end-pytorch-training-submission)
* `epochs=400`, `T_max=5`, `batch_size=256`
* `CV:0.52`  , `LB:0.19`

## Version5
* No ArcFace
* StratifiedGroupKFold for validation
* Great feature generation using PyTorch model based on this [notebook](https://www.kaggle.com/code/mayukh18/end-to-end-pytorch-training-submission)
* `epochs=300`, `T_max=10`, `batch_size=128`
* `CV:0.51`  , `LB:0.19`

## Version6
* No ArcFace
* Model from [🤟 GISLR 🤟 - 📚Learn – 🔭EDA – 🤖Baseline](https://www.kaggle.com/code/dschettler8845/gislr-learn-eda-baseline)
* StratifiedGroupKFold for validation
* Great feature generation using PyTorch model based on this [notebook](https://www.kaggle.com/code/mayukh18/end-to-end-pytorch-training-submission)
* `epochs=300`, `T_max=10`, `batch_size=128`
* `CV:0.48`  , `LB:0.50`

## Version7
* No ArcFace
* Model from [🤟 GISLR 🤟 - 📚Learn – 🔭EDA – 🤖Baseline](https://www.kaggle.com/code/dschettler8845/gislr-learn-eda-baseline)
* StratifiedGroupKFold for validation
* Great feature generation using PyTorch model based on this [notebook](https://www.kaggle.com/code/mayukh18/end-to-end-pytorch-training-submission) and my [notebook](https://www.kaggle.com/code/medali1992/isolated-sign-language-aggregation-preparation) for feature generation.
* Removed the 'z' axis and face features and rerplaced them with lips as stated [here.](https://www.kaggle.com/competitions/asl-signs/discussion/391812)
* `epochs=500`, `T_max=10`, `batch_size=512`, `num_blocks=3`
