---
layout: post
title: What is Back Propagation? How Can we improve it? 
---
Introduction to Basic working of Backpropagation, Mean Squared Error, Bias Vs Variance.

## A Learning Machine

 There are several approaches to Machine Learning, But many of the successful approaches can be categorised as <b> Gradient Based Methods</b>, It can be visualized as a machine where the inputs are Z0, Z1, Z2, Z3, .... Zp and there are some Tweakable Parameters W which are given as input to the Learning Machine M(Z,W), and the output of this is then compared to the Cost Function, which has the Out put to these Learning Machine and the Desired Output, So Basically these cost Fuctions Ep = C (Dp, M(Zp, W)); 
 Where Ep is the Output of the Cost fuction, C is the Cost Fucntion, Dp is the Desired Output and M (Zp ,W) is the output of the Learning Machine,

 <p> In laymans term, the problems boils down to just decreasing the Value of the Output of the cost Function by tweaking  the W parameters, 

 <p> The Most commonly used cost function is the Mean Squared Error: Ep = 1/2(Dp - M(Zp,W))^2,
 	Etrain = 1/p(SUM p=1 Ep),

<p> We always dont want to Error to be Zero because then the Machine Looses it's Generality, should always try to maximize the ability of the Network to <i>generalize</i>, That is to predict the correct targets for patterns the learning system has not previously seen before. For Example if we took multiple Samples each of the samples will have different noises, then and we train the Network such that the Cost Fucntion outputs very less error and then the machine even tends to Learn the noise that Particular Dataset on which the dataset have been trained upon. And this totally goes against the sole purpose that is maximizing the generalization of the Machine. There are Generalization Techniques that try to correct for the errors introduced into the networkas a result of our choice of dataset. Both minimizing the error and improvising the generalization of the Machine are important.

### Bias Vs Variance

 <p> As Stated previously It is important to both reduce the Output of the Cost Function and also not reduce the so much so the we tend to Over train the network, a stage where the Learning machine Learns the Noise of the Data Set, so It is also important to Increase the Generalization of the Learing Machine.

 <p> So there are Two terms <B> BIAS </b> and <b> VARIANCE </b>,

 	Bias is a measure of how much the network output, averaged over all possible data sets differs from the desired function.