# ACGANs Improve Chemical Sensors for Challenging Distributions
Public repo corresponding to ACGANs Improve Chemical Sensors for Challenging Distributions - ICMLA 2022 Oral Presentation + Paper

Images, tables, abstract, description. Can't provide data due to Defense Threat Reduction Agency project

## Primary results
![results table 1](imgs/table1.png)


![results table 2](imgs/table2.png)

- An ablation study on synthesis of [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) proposing three novel architectures for conditional data generation which demonstrate improvement on baseline generation quality for a natural image dataset as well as increasingly small subsets across multiple generative metrics.

- A novel approach to structure latent representations by learning a paired structured condition space and weakly structured variation space with desirable sampling and supervised learning properties. 

- A discussion of conditional image synthesis metrics with a comparison to alternative methods for evaluating the quality of conditionally-generated images. 

The alterations to include cycles in conditional generators demonstrate improvements to comparable baseline CGANs across a variety of established and proposed metrics. Additional experiments demonstrate the successes of inducing cycles in conditional GANs for both image synthesis and image classification over comparable models.

![imageLeft](imgs/analyte_a.png)

![imageLeft](imgs/analyte_b.png)

## Novelty
We induce cycles for conditional generators to move samples between labelled latent and data spaces such that the generative quality and supervised learning ability of the resulting model is improved.

Conditional Autoencoder-GAN             |  Cycle Conditional Autoencoder-GAN
:-------------------------:|:-------------------------:
![imageLeft](imgs/CAEGAN_annot.png)  |  ![imageRight](imgs/CCAEGAN_annot.png)


