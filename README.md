# ACGANs Improve Chemical Sensors for Challenging Distributions
Public repo corresponding to ACGANs Improve Chemical Sensors for Challenging Distributions - ICMLA 2022 Oral Presentation + Paper

Training machine learning models to remain accurate on distribution-shifted testing data requires performing many diverse, costly experiments in controlled laboratory settings to create a well-rounded training data set. In practice even expensive, large data sets may be insufficient for generalization of a trained model to a real-world testing distribution. It is possible but costly to create large, diverse datasets of single-analyte exposures, but experimentation with multi-analyte combinations quickly becomes intractable.

With this in mind, we benchmark and propose machine learning and deep learning approaches to the detection of obscured chemical analytes given only single-analyte training. We significantly improve upon baseline classification of a particular chemical analyte borne in vapor mixed with an obscurant chemical agent by inducing multitask learning through adversarial data synthesizing models.

Given chemical analyte exposure times between 0.75 and 5 seconds and across three unique experiment data sets comprised of different sensors and experimental controls, we find approaches utilizing Auxiliary Classifier Generative Adversarial Networks (ACGANs) outperform machine learning and comparable neural network approaches. We corroborate with multitask learning to find that across domains the utilization of generative tasks in supervised learners may increase data efficiency and model robustness to out-of-distribution samples without additional data annotation.

## Primary results
![results table 1](imgs/table1.png)


![results table 2](imgs/table2.png)

- An ablation study on synthesis of [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) proposing three novel architectures for conditional data generation which demonstrate improvement on baseline generation quality for a natural image dataset as well as increasingly small subsets across multiple generative metrics.

- A novel approach to structure latent representations by learning a paired structured condition space and weakly structured variation space with desirable sampling and supervised learning properties. 

- A discussion of conditional image synthesis metrics with a comparison to alternative methods for evaluating the quality of conditionally-generated images. 

The alterations to include cycles in conditional generators demonstrate improvements to comparable baseline CGANs across a variety of established and proposed metrics. Additional experiments demonstrate the successes of inducing cycles in conditional GANs for both image synthesis and image classification over comparable models.

![imageLeft](imgs/analyte_a.png)

![imageRight](imgs/analyte_b.png)

## Novelty
We induce cycles for conditional generators to move samples between labelled latent and data spaces such that the generative quality and supervised learning ability of the resulting model is improved.

Conditional Autoencoder-GAN             |  Cycle Conditional Autoencoder-GAN
:-------------------------:|:-------------------------:
![imageLeft](imgs/CAEGAN_annot.png)  |  ![imageRight](imgs/CCAEGAN_annot.png)


