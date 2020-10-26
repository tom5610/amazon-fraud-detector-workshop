# Amazon Fraud Detector Workshop Lab
---

The repository is based https://github.com/mikames/data-and-notebooks and I've added the model training and merge prediction with Mike's prediction notebook. I hope that you enjoy the learning.

## Steps

* Spin up environments with [fraud-detector-workshop.yaml](./fraud-detector-workshop.yaml), which creates:
  * Amazon SageMaker Notebook instance
  * IAM roles for Notebook instance and Amazon Fraud Detector data access
* Open Jupyter notebook from SageMaker Notebook instance and start experiencing model training and prediction with Fraud Detector.

## Estimated Cost of Running the Workshop

If the workshop is being done on a new AWS account or an account without using Amazon SageMaker & Amazon Fraud Detector before, the two month free tier offering should be able to cover the cost. For more detail about free tier / free trial: [Amazon SageMaker](https://aws.amazon.com/sagemaker/pricing/) & [Amazon Fraud Detector](https://aws.amazon.com/fraud-detector/pricing/)

### Assumption:
* Estimated Cost: 0.39 * 1 + 0.06 * 1.5 + 0.03 * 1000 + 0.0739 * 1.5 = ***$31.5USD***
  * The workshop takes approx. 1.5 hours.
  * 25MB data file is stored in S3 bucket tempoarily (with which the cost can be ignored).
  * Only one model version is created with train data set - [project_1_newaccounts_100k.csv](./project_1_newaccounts_100k.csv), which takes approx. 1hr. And the model hosting time is approx. 1.5 hours.
  * Approx 1,000 times of fraud predictions will be invoked.
  * 1 hours usage of t3.medium of Amazon SageMake Notebook instance in Sydney Region ($0.0739 USD per hour)

## Notes
This repository contains sample notebooks and data, feel free to use as you like. 
