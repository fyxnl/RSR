 
# Towards Real-World Scene Recovery: Benchmark and Method

This is the official PyTorch implementation of RSR
## Abstract:
Restoring images in haze and sandstorm scenes is a challenging but widely concerned topic in computer vision. The mainstream learning-based approaches primarily obtain the enhanced model by relying on the distribution of training data from the specific scenes, causing poor generalization when encountering previously unseen real-world degraded images.
The primary difficulty stems from the domain gap caused by diverse real-world degradation factors (e.g., haze, low light, noise, color cast), which are often absent in previous synthetic haze and sandstorm data. To bridge this gap, we first conduct statistical analysis of visual and physical properties across various real haze and sandstorm scenes and construct a multi-domain data generation pipeline that simulates representative conditions such as daytime haze, nighttime haze, and dusty weather. This allows our model to learn from richer degradation patterns and better generalize across scenes.
We then introduce a two-stage domain adaptation paradigm that models the domain shift via subspace domain alignment and domain-invariant feature learning. In the first supervised phase, we remove the spurious correlation between features by learning the weights of the source domain sample data in the representation space, so as to obtain domain invariant features. In the second unsupervised phase, we align second-order feature statistics to minimize domain discrepancy in the transformed subspace. Finally, extensive experiments and ablation studies on multiple challenging haze and sandstorm data indicate our method's superiority in image quality and scenario adaptability against existing state-of-the-art methods. Applications on vehicle object detection also reveal the latent practical values for the proposed method. 

![](Fig/1.png)
## Environment:

- Windows: 10

- CUDA Version: 11.0 
- Python 3.7

## Dependencies:

- torch==1.7.0
- torchvision==0.7.0
- NVIDIA GPU and CUDA

## Pretrained Weights & Dataset

1. Download [Dehaze weights](https://pan.baidu.com/s/1N5DuuqQEyAUtk8Ec6tLCpw?pwd=tib6) and Extraction code: [tib6]
2. Load the pre-trained weights [Res2Net](https://pan.baidu.com/s/14JAHqX0xvFTpGXAqVBqMCQ) and Extraction code: [1234]
3. Our training data will be released once it's sorted out. Data layer generalization can be achieved with our data.
![](USfigure/6.png). 

## train
Our training code will be released once it's sorted out.

 

## Test

Our test run is simple, just change the input and output paths according to your requirements

```
python TMM_test.py
```

## Qualitative Results
![](Fig/2.png)
 
 

## Acknowledgement

**

 
## Citation

**



 
