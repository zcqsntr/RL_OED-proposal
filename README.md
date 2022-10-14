# Deep Reinforcement Learning for Optimal Experimental Design in Biology

A proposal by Neythen Treloar etc.

## Abstract


The field of optimal experimental design uses mathematical techniques to determine experiments that are maximally informative from a given experimental setup. Here we apply a technique from artificial intelligence—reinforcement learning—to the optimal experimental design task of maximizing confidence in estimates of model parameter values. We show that a reinforcement learning approach performs favourably in comparison with a one-step ahead optimisation algorithm and a model predictive controller for the inference of bacterial growth parameters in a simulated chemostat. Further, we demonstrate the ability of reinforcement learning to train over a distribution of parameters, indicating that this approach is robust to parametric uncertainty.

## Introduction and Prior Work


Biological systems are often complex and typically exhibit non-linear behaviour, making accurate model parametrisation difficult. Optimal experimental design tools help address this problem by identifying experiments that are predicted to provide maximally informative data for parameter inference. In [previous work](https://www.biorxiv.org/content/10.1101/2022.05.09.491138v1.abstract) we used reinforcement learning to determine such experiments. Our simulation studies show that this approach allows uncertainty in model parameterisation to be directly incorporated into the search for optimal experiments, opening a practical avenue for training an experimental controller. 
The current state of the work is that the method has been demonstrated on a couple of relatively simple models and there are some compelling reasons to use RL over more traditional optimisation based approaches, mainly fast online decision making and the ability to easily incorporate parameter/model uncertainty. This work caught the interest of Nicolas Cruz at Technische Universität Berlin as they are limited by the slow speed of traditional approaches and we have instigated a collaboration to implement this into their high throughput lab setup in the near future. 

A key future direction for this work will be investigating the scale up to more complex models and more complex OED tasks such as simultaneous model discrimination and parameter inference and this will be the main aim of the proposed project. Theogical community. method has already been developed and demonstrated so the main focus of this would be engineering the RL up to a larger scale in the best way. A secondary goal would be to develop an easy to use python package so that the method can be cessable to non-experts and help increase the dissemination of machine leanring into the biological community. 

## Deliverables

### Paper

Can the project be turned into a paper? What does the evaluation process for such a paper look like? What conferences are we targeting? Can we release a blog post as well as the paper?


There is a clear route to publication and the wide ranging interest of the scientific community in this method has already been proven (the work has been accepted and presented at two conferences across different disciplines (AI4synbio and the mediterrain conference on control)). 

### Software Package

The work could be released as a software package with the aim to make the implementation of the OED method accessible for use by non-experts. With a collaboration that has already been initiated we can test the package in a high throughput biological laboratory. 

## Resources

### Requirements

What kinds of resources (e.g. GPU hours, RAM, storage) are needed to complete the project?

### Timeline

6 months to 1 year

## Broader Impact

How is the project expected to positively impact biological research at large?

## Reproducibility

All code can be published publically on GitHub, with working examples to run on various models. 

## Failure Case

If our findings are unsatisfactory, do we have an exit plan? Do we have deliverables along the way that we can still provide the community with?

## Preliminary Findings

We had written a [paper](https://www.biorxiv.org/content/10.1101/2022.05.09.491138v1.abstract), currently on bioArxiv, in review at PLOS computational biology which demonstrates the effectiveness of the method on simple models. Based on this paper we were contacted by Nicolas Cruz group to initiate a collaboration to implement our method in their lab. 


## Next Steps

If the project is successfully completed, are there any obvious next steps?

## Known contributors

Neythen Treloar, Postdoctoral Research Fellow, University College London
