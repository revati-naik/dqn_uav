## Uncertainty Estimation in Deep Learning Networks


This is the code sample to implement the deep learning model with ResNet18 Architecture and ADF layers to calculate the uncertainty and provide a confidence score. 



### Prerequisites

  * torch 1.4.0
  * torchvision 0.5.0


### Data

The code uses CIFAR-10 data set to train and run the evaluation. The dataset is automatically downlaoded in teh code script.

### Training

Resume the training using

python train.py -r --model_name resnet18

### Evaluation

Evaulate/test the model using

    python3 eval.py -r -b -m --load_model_name resnet18 --test_model_name resnet18_adf --p 0.02 --min_variance 1e-3 --noise_variance 1e-3


