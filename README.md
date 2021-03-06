# LGN

We attempt to build a Lorentz Group Equivariant Network (LGN); an ML model which respects symmetries in high energy physics, for the task of jet classification.

This work is based on this repository: https://github.com/fizisist/LorentzGroupNetwork

## Abstract
Neural networks which are Lorentz group equivariant are extremely desirable for high energy physics data. In this work, we attempt to build such a model and train it to the task of jet-classification. The model reaches state-of-the-art performance, in addition to passing a series of physics equivariance tests; suggesting a new realm of experimentation with physics equivariant models.


## Training Result
We have trained the LGN model for 20 epochs and here are our loss plots:
<img src="pics/loss.png" alt=loss width="480"/>


Here are our accuracy plots:

<img src="pics/acc.png" alt=acc width="460"/>


## MODEL EVALUATION
### Ml Metrics (Roc curves & Confusion Matrix)


<p float="left">
  <img src="pics/ROC.png" alt="ROC" width="430"/>
  <img src="pics/ConusionMatrix.png" alt="ConusionMatrix" width="350"/>
</p>



### Physics Metrics

<p float="left">
  <img src="pics/RotInv.png" alt="RotInv" width="370"/>
  <img src="pics/BoostInv.png" alt="BoostInv" width="420"/>
</p>



## Conclusion

- We have achieved a benchmark test accuracy of 92.7% at epoch number 19, which is comparable to the test accuracy they have achieved in the paper [1] of around 92.9%.


- We have achieved an AUC of 96.9% which is higher than the AUC achieved in the paper [1] by the LGN model (96.4%). This result is really nice considering our resources and the time constraint we had to produce this work.

- We have showed how the LGN model is fully equivariant w.r.t Lorentz symmetries


## Main reference: 
[1] https://arxiv.org/pdf/2006.04780.pdf

## Other references: 
https://scipost.org/10.21468/SciPostPhys.5.3.028

https://mcgreevy.physics.ucsd.edu/f20/final-papers/2020F-220-Kansal-Raghav.pdf
