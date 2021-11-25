# Epilepsy-Domain-Adversarial-Neural-Network


## Paper link: [Epilepsy SEEG Data Classification Based On Domain Adversarial Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9447726)

## Abstract
Epilepsy is a neurological disorder characterized by recurrent epileptic seizures. Although an increasingly intense research effort has focused on the use of brain signal data to predict or detect epileptic seizures as early as possible, this problem is still computationally challenging. The main challenge is that the patient’s brain signal has strong individual characteristics, and the classification model is easily disturbed by this, which may lead to false predictions, affecting the reliability of the model. Based on the development of brain signal acquisition technology and deep learning, we propose a new type of deep learning model called the Epilepsy Domain Adversarial Neural Network (EDANN) model, which is used to classify epileptic pre-ictal signals. EDANN integrates multiple deep neural networks based on the idea of adversarial learning, which can reduce the impact of the differences between patients on model prediction. The multi-network design in EDANN effectively improves the model training stability and model generalizability. In addition, a unique brain signal processing algorithm is developed to convert signals to data blocks that are ready for pre-ictal classification, and the model may provide an auxiliary diagnosis for early warning of epilepsy. Experimental results on real patient data show that EDANN clearly improved the F1 score by approximately
7.2% compared with the existing models. On a real dataset, our model achieved state-of-the-art results.



## Project

we propose a new type of deep learning model called Epilepsy Domain Adversarial Neural Network model (EDANN), which is used to classify epileptic pre-ictal signals. EDANN integrates multiple deep neural networks, based on the idea of adversarial learning, which can reduce the impact of differences between patients on model prediction. The multi-network design in EDANN effectively improves the model training stability and model generalizability. 

## Environment

The model built by Pytoch framework, Python3.6. You May need to install these packages as follows: 

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

Due to wo need permission to disclose data. If we get permission, we will disclose data later.

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

Training  EDANN-LSTM model by:

```
python ./run.py -m train -lac LSTM -p patient_name -gpu 0 -ep 30 -bs 64
```

Test EDANN-LSTM model by:

```
python ./run.py -m test -lac LSTM -p patient_name -gpu 0 
```

## Tips
If you want to see more detail, you can see link https://github.com/danzhewuju/ANNSD. It contains full code about our work. I hope it can help you.
