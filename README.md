# Epilepsy-Domain-Adversarial-Neural-Network



## Project

we propose a new type of deep learning model called Epilepsy Domain Adversarial Neural Network model (EDANN), which is used to classify epileptic pre-ictal signals. EDANN integrates multiple deep neural networks, based on the idea of adversarial learning, which can reduce the impact of differences between patients on model prediction. The multi-network design in EDANN effectively improves the model training stability and model generalizability. 

## Environment

The model built by Pytoch framework, Python3.6. You May need to install  these 

packages as follows: 

dtw               1.4.0

mne               0.23.dev0

numpy             1.19.5

opencv-python     4.5.1.48

pandas            1.2.0

pyEDFlib          0.1.20

pyparsing         2.4.7

python-dateutil   2.8.1

scikit-learn      0.24.0

scipy             1.6.0

torch             1.7.1

torchvision       0.8.2

tqdm              4.56.0

## Data

We need permission to disclose data.

## How to run?

You can use shell to run code, and you need go to "mymodel" dir.

Training  EDANN-Transformer model by:

```
python ./run.py -m train -lac Transformer -p patient_name -gpu 0 -ep 30 -bs 64
```

Test EDANN-Transformer model by:

```
python ./run.py -m test -lac Transformer -p patient_name -gpu 0 
```

