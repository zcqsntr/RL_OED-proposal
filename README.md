# Deep Reinforcement Learning for Optimal Experimental Design in Biology

A proposal by Neythen Treloar etc.

## Abstract


The field of optimal experimental design uses mathematical techniques to determine experiments that are maximally informative from a given experimental setup. Here we apply a technique from artificial intelligence—reinforcement learning—to the optimal experimental design task of maximizing confidence in estimates of model parameter values. We show that a reinforcement learning approach performs favourably in comparison with a one-step ahead optimisation algorithm and a model predictive controller for the inference of bacterial growth parameters in a simulated chemostat. Further, we demonstrate the ability of reinforcement learning to train over a distribution of parameters, indicating that this approach is robust to parametric uncertainty.

## Introduction and Prior Work


Biological systems are often complex and typically exhibit non-linear behaviour, making accurate model parametrisation difficult. Optimal experimental design tools help address this problem by identifying experiments that are predicted to provide maximally informative data for parameter inference. In [previous work](https://www.biorxiv.org/content/10.1101/2022.05.09.491138v1.abstract) we used reinforcement learning to determine such experiments. Our simulation studies show that this approach allows uncertainty in model parameterisation to be directly incorporated into the search for optimal experiments, opening a practical avenue for training an experimental controller. 
The current state of the work is that the method has been demonstrated on a couple of relatively simple models and there are some compelling reasons to use RL over more traditional optimisation based approaches, mainly fast online decision making and the ability to easily incorporate parameter/model uncertainty. We should also be working with Nicolas Cruz at Technische Universität Berlin to implement this into their high throughput lab setup in the near future. They read our preprint and became very interested, primarily as they are finding themselves limited by the slow speed of the optimisation approaches.

A key future direction for this work will be investigating the scale up to more complex models and more complex OED tasks such as simultaneous model discrimination and parameter inference, I think this is where OpenBioML could really help. Basically we would want to find out how far we can scale up the method and what would be the best ways to scale up the RL so that this is possible. The method has already been developed and demonstrated so the main focus of this would be engineering the RL up to a larger scale in the best way. I think this is a very well defined problem, already with compelling use cases and a clear path to real life implementation, so I think it could be a relatively 'easy win' for OpenBioML

## Deliverables

### Software Package

The work could be released as a software package with the aim to make the implementation of the OED method accessible for use by non-experts. With a collaboration that has already been initiated we can test the package in a high throughput biological laboratory. 

### Paper

Can the project be turned into a paper? What does the evaluation process for such a paper look like? What conferences are we targeting? Can we release a blog post as well as the paper?


There is a clear route to publication and the wide ranging interest of the scientific community in this method has already been proven (the work has been accepted and presented at two conferences across different disciplines (AI4synbio and the mediterrain conference on control)). 

## Resources

### Requirements

What kinds of resources (e.g. GPU hours, RAM, storage) are needed to complete the project?

### Timeline

What is a (rough) timeline for this project?

## Broader Impact

How is the project expected to positively impact biological research at large?

## Reproducibility

What steps are going to be taken to ensure the project's reproducibility? Will data processing scripts be released? What about training logs?

## Failure Case

If our findings are unsatisfactory, do we have an exit plan? Do we have deliverables along the way that we can still provide the community with?

## Preliminary Findings

If applicable, mention any preliminary findings (e.g. experiments you have run on your own or heard about) that support the project's importance.

## Next Steps

If the project is successfully completed, are there any obvious next steps?

## Known contributors

Please list community members that you know are interested in contributing. It is best if a project proposal already has an associated team capable of going ahead with the project by themselves, but it is not necessary.
