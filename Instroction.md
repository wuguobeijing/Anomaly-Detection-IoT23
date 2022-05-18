# dataset
## dataset1
Data Preprocessing/iot23_combined.csv

2739674 rows
part of iot-23
unbalance

## dataset2
## Models/iot23_combined_oversample.csv
4725417 rows
part of iot-23
balanced dataset1

Models/Data/split
## Models/Data/split/test_data.csv
30287 rows
part of Models/Data/iot23_all_combined.csv

## Models/Data/split/test_data_big.csv

part of ./Data/iot23_all_combined_big.csv

## Models/Data/split/test_data_big_balance.csv
1562764 rows
part of iot23_all_combined_big_balance.csv

## Models/Data/split/test_data_ToN_big_balance.csv
118971 rows
part of Models/Data/ToN-iot_all_combined_big_balance.csv

## Models/Data/split/ToN-iot-test_data.csv
92209 rows
part of Models/Data/ToN-iot_all.csv

## Models/Data/split/ToN-iot-train_data.csv
368834 rows
part of Models/Data/ToN-iot_all.csv

## Models/Data/split/train_data.csv
121148 rows
part of Models/Data/iot23_all_combined.csv

## Models/Data/split/train_data_big.csv

part of ./Data/iot23_all_combined_big.csv

## Models/Data/split/train_data_big_balance.csv
6251056 rows
part of iot23_all_combined_big_balance.csv

## Models/Data/split/train_data_ToN_big_balance.csv
475881 rows
part of Models/Data/ToN-iot_all_combined_big_balance.csv


Models/Data/test
## Models/Data/test/ALL
each file is a part of original senario files

Models/Data/test/iot23_all_combined_test.csv
Models/Data/test/iot23_attack_combined_test.csv
Models/Data/test/iot23_Benign_combined_all.csv
Models/Data/test/iot23_Benign_combined_test.csv
##Models/Data/test/ToN-iot_test.csv
random pick

## Models/Data/iot23_all_combined.csv
about 2800000 rows
unbalanced data 

## Models/Data/iot23_all_combined_big.csv
4286300 rows
part of iot-23 
unbalanced

## Models/Data/iot23_all_combined_big_balance.csv
7813820 rows
（each type with a num around 3840000）
balanced by SOMO

## Models/Data/iot23_attack_combined.csv
3906910 rows
take sample from each file of BigDataset/attacks

## Models/Data/iot23_attack_combined_big.csv
same as Models/Data/iot23_all_combined_big_balance.csv

## Models/Data/iot23_Benign_combined.csv
all the benign data from original senarios

## Models/Data/iot23_Benign_combined_big.csv
all the benign data from original senarios(bigger)

## Models/Data/ToN-iot_1_all.csv
first file of ToN-iot

## Models/Data/ToN-iot_all.csv
461043 rows
from Train_Test_Network.csv

## Models/Data/ToN-iot_all_combined_big_balance.csv
594852 rows
part of ToN
balanced by SMOTE_ENN

# processed result
## Models/AdB

Models/IoT23 - AdaBoost(self).ipynb

## Models/DT

Models/IoT23 - DecisionTrees(self).ipynb
Models/IoT23 - DecisionTrees.ipynb
Models/IoT23 - DecisionTrees_mul(self).ipynb

## Models/RF

Models/IoT23 - RF(self).ipynb
Models/IoT23 - RF_mul(self).ipynb

## Models/STACKING

Models/iot23-stacking.ipynb

## Models/XGB

Models/IoT23 - XGB(self).ipynb
Models/IoT23 - XGB_MUL(self).ipynb

## Models/Other_model

Models/IoT23 - CNN(self).ipynb
Models/IoT23 - CNN.ipynb
Models/IoT23 - CNN_mul(self).ipynb
Models/IoT23 - SVM(self).ipynb
Models/IoT23 - SVM.ipynb
Models/IoT23 - Naive Bayes(self).ipynb
Models/IoT23 - Naive Bayes.ipynb

**above models are trained with the dataset2**

## Models/auto_gl.ipynb

use auto-gluon to train models with different complexity,fine-tuned model is the model to generate models that can be
easily deploy on edge device.

## Models/sampling.ipynb

use for downsampling and balance data(both iot23 and ToN-iot)

## Models/sampling_balance_malware.ipynb

balance different type of malicious(failed for the total count of total count,maybe try to downsampling the majority to 5000)

## Models/sampling_test.ipynb
 make test data for iot23(decided not to use)