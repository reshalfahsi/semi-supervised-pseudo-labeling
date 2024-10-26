# Semi-Supervised Learning with Pseudo-Labeling


<div align="center">
    <a href="https://colab.research.google.com/github/reshalfahsi/semi-supervised-pseudo-labeling/blob/master/Semi_Supervised_Learning_with_Pseudo_Labeling.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="colab"></a>
    <br />
</div>


The need for semi-supervised learning stems from the cost of annotating datasets. Datasets do not always come with fully labeled data. Henceforth, we can cleverly perform compound training with labeled and unlabeled data. One of the semi-supervised methods we can employ is pseudo-labeling. At first, we train our model with labeled data and generate labels for unlabeled data based on it. Next, we train the pre-trained model with both labeled and unlabeled data. This is possible due to pseudo-labels generated earlier. In this project, DenseNet-121 is utilized. The model is trained on CIFAR-10 with 1000 labels.


## Experiment

To cater to your curiosity, you can catch the implementation [here]((https://github.com/reshalfahsi/semi-supervised-pseudo-labeling/blob/master/Semi_Supervised_Learning_with_Pseudo_Labeling.ipynb).



## Result

## Quantitative Result

Refer to the table below to discern the quantitative results.

Test Metric | Score |
----------- | ----- |
Accuracy | 62.77 %
Loss | 1.274


## Accuracy and Loss Curves

### Labeled Data

<p align="center"> <img src="https://github.com/reshalfahsi/semi-supervised-pseudo-labeling/blob/master/assets/labeled_loss_curve.png" alt="labeled_loss_curve" > <br /> The loss curve on the labeled train and validation sets of the model. </p>

<p align="center"> <img src="https://github.com/reshalfahsi/semi-supervised-pseudo-labeling/blob/master/assets/labeled_acc_curve.png" alt="labeled_acc_curve" > <br /> The accuracy curve on the labeled train and validation sets of the model. </p>

### Labeled and Unlabeled Data

<p align="center"> <img src="https://github.com/reshalfahsi/semi-supervised-pseudo-labeling/blob/master/assets/labeled_unlabeled_loss_curve.png" alt="labeled_unlabeled_loss_curve" > <br /> The loss curve on the labeled and unlabeled train and validation sets of the model. </p>

<p align="center"> <img src="https://github.com/reshalfahsi/semi-supervised-pseudo-labeling/blob/master/assets/labeled_unlabeled_acc_curve.png" alt="labeled_unlabeled_acc_curve" > <br /> The accuracy curve on the labeled and unlabeled train and validation sets of the model. </p>


## Qualitative Result

This 3 × 3 image grid shows the qualitative results on the test set.


<p align="center"> <img src="https://github.com/reshalfahsi/semi-supervised-pseudo-labeling/blob/master/assets/qualitative.png" alt="qualitative" > <br /> The grid of qualitative results. </p>



## Credit

- [The CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html)
- [Learning Multiple Layers of Features from Tiny Images](https://www.cs.toronto.edu/~kriz/learning-features-2009-TR.pdf)
- [Pseudo-Label : The Simple and Efficient Semi-Supervised Learning Method for Deep Neural Networks](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=798d9840d2439a0e5d47bcf5d164aa46d5e7dc26)
- [Densely Connected Convolutional Networks](https://arxiv.org/pdf/1608.06993)
- [PyTorch Lightning](https://lightning.ai/docs/pytorch/latest/)
