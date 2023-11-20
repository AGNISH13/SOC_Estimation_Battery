# State-Of-Charge estimation from "LG 18650HG2 Li-ion Battery Data"

## Project Description
This is a python-based project predicting the `SOC` of the `Li-ion Battery` in Electric Vehicles (EV) based on `Regression` technique utilizing a two-layer `Convolutional Neural Network`. The entire coding workflow can be viewed in the ipynb file present in this repository.
This project has been inspired from [this repository](https://github.com/sautee/battery-state-of-charge-estimation/tree/main).

## Dataset Description
The models are built using Tensorflow and trained on the [LG18650HG2](https://data.mendeley.com/datasets/cp3473x7xv/3) Li-ion Battery Dataset.
(Kollmeyer, Philip; Vidal, Carlos; Naguib, Mina; Skells, Michael (2020), “LG 18650HG2 Li-ion Battery Data and Example Deep Neural Network xEV SOC Estimator Script”, Mendeley Data, V3, doi: 10.17632/cp3473x7xv.3)

Format in which the data has been stored while training using the model can be viewed [here](https://drive.google.com/drive/folders/1fwOdWS7FWJw0zuVVotXa_1kmB0fOGEgg).

## Results
The data has been trained and tested on the [original model](https://github.com/sautee/battery-state-of-charge-estimation/blob/main/training/lg/lg_cnn_minmaxnorm_1Hz_conv1d.ipynb) previously used on this dataset as well as our proposed model. Given below is the comparison of the results using both.

Loss Plots:
-     Original Model
     ![image](https://github.com/AGNISH13/SOC_Estimation_Battery/assets/84792746/9c984174-1365-4fb2-a1c2-38f06a72ba98)
-     Proposed Model
     ![image](https://github.com/AGNISH13/SOC_Estimation_Battery/assets/84792746/52b99ab6-9255-40a7-98bc-0f227a6c5848)

Predicted SOC vs True SOC:
-     Original Model
     ![image](https://github.com/AGNISH13/SOC_Estimation_Battery/assets/84792746/7e9a422c-b71f-4f1f-9478-e23b33bbae62)
-     Proposed Model
     ![image](https://github.com/AGNISH13/SOC_Estimation_Battery/assets/84792746/40e489d7-2b1a-4aec-a11c-781bf383eff1)

Prediction Error Distribution:
-     Original Model
     ![image](https://github.com/AGNISH13/SOC_Estimation_Battery/assets/84792746/bdffac8d-d888-402c-85cd-65d663e5c158)
-     Proposed Model
     ![image](https://github.com/AGNISH13/SOC_Estimation_Battery/assets/84792746/df58af2b-f058-4165-9d6e-eafdadf60d79)

Scatter Plots on Test Dataset:
-     Original Model
     ![Newplot_Original](https://github.com/AGNISH13/SOC_Estimation_Battery/assets/84792746/fe589713-c030-432b-95ab-1209a3c59d76)
-     Proposed Model
     ![Newplot_Proposed](https://github.com/AGNISH13/SOC_Estimation_Battery/assets/84792746/56f1263d-a3db-42c4-a843-62985e71c3db)

## Dependencies
This entire project is based on `Python` programming language. The models have been trained and tested entirely using the resources `Google Colab`.
The Python packages which are in use in this project are  `matplotlib`, `numpy`, `pandas`, `datetime`, `os`, `sys`, `tensorflow` and `keras`.

## Acknowledgements
https://github.com/sautee/battery-state-of-charge-estimation

Kollmeyer, Philip; Vidal, Carlos; Naguib, Mina; Skells, Michael (2020), “LG 18650HG2 Li-ion Battery Data and Example Deep Neural Network xEV SOC Estimator Script”, Mendeley Data, V3, doi: 10.17632/cp3473x7xv.3

D. N. T. How, M. A. Hannan, M. S. H. Lipu, K. S. M. Sahari, P. J. Ker and K. M. Muttaqi, "State-of-Charge Estimation of Li-ion Battery in Electric Vehicles: A Deep Neural Network Approach," 2019 IEEE Industry Applications Society Annual Meeting, Baltimore, MD, USA, 2019, pp. 1-8, doi: 10.1109/IAS.2019.8912003
