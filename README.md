# Amazon Fraud Detector Workshop Lab
---

The repository is based https://github.com/mikames/data-and-notebooks and I've added the model training and merge prediction with Mike's prediction notebook. I hope that you enjoy the learning.

## Steps

* Spin up environments with [fraud-detector-workshop.yaml](./fraud-detector-workshop.yaml), which creates:
  * Amazon SageMaker Notebook instance
  * IAM roles for Notebook instance and Amazon Fraud Detector data access
* Open Jupyter notebook from SageMaker Notebook instance and start experiencing model training and prediction with Fraud Detector.

## Cost
* Assumption:
  * Training data storage cost on S3 is so tiny can be ignored. (25MB data file is stored tempoarily.)
  * Only one model version is created with train data set - [project_1_newaccounts_100k.csv](./project_1_newaccounts_100k.csv), which takes approx. 1hr. And the model hosting time is approx. 6 hours.
  * Approx 1,000 time of fraud predictions will be invoked.
* Pricing: 0.39 * 1 + 0.06 * 6 + 0.03 * 1000 = ***$30.75 USD***

## Notes
This repository contains sample notebooks and data, feel free to use as you like. 
