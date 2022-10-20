# Deep Reinforcement Learning for Optimal Experimental Design in Biology

A proposal by Neythen Treloar etc.

## Abstract


The field of optimal experimental design uses mathematical techniques to determine experiments that are maximally informative from a given experimental setup. In previous work we have applied reinforcement learning to the optimal experimental design task of maximizing confidence in estimates of model parameter values for some simple biological models. We have shown that a reinforcement learning approach performs favourably in comparison with a one-step ahead optimisation algorithm and a model predictive controller for the inference of bacterial growth parameters in a simulated chemostat. Further, we demonstrated the ability of reinforcement learning to train over a distribution of parameters, indicating that this approach is robust to parametric uncertainty.

Here we propose to undertake a key future direction for this work; investigating the scale up to more complex models and more complex OED tasks such as simultaneous model discrimination and parameter inference, and this will be the main aim of the proposed project. The method has already been developed and demonstrated so the main focus of this would be engineering the RL up to a larger scale in the best way and demonstrating it effectiveness on a number of large scale biological models. A secondary goal would be to develop an easy to use python package so that the method can be cessable to non-experts and help increase the dissemination of machine leanring into the biological community. 


## Introduction and Prior Work

- Our paper can be found [here](https://www.biorxiv.org/content/10.1101/2022.05.09.491138v1.abstract). See this for a thorough introduction with lots of references. 

Biological systems are often complex and typically exhibit non-linear behaviour, making accurate model parametrisation difficult. Optimal experimental design tools help address this problem by identifying experiments that are predicted to provide maximally informative data for parameter inference. In this work we used reinforcement learning to determine such experiments. Our simulation studies show that this approach allows uncertainty in model parameterisation to be directly incorporated into the search for optimal experiments, opening a practical avenue for training an experimental controller. 
The current state of the work is that the method has been demonstrated on a couple of relatively simple models and there are some compelling reasons to use RL over more traditional optimisation based approaches, mainly fast online decision making and the ability to easily incorporate parameter/model uncertainty. 


## Deliverables

### Paper

There is a clear route to publication and the wide ranging interest of the scientific community in this method has already been proven (the work has been accepted and presented at two conferences across different disciplines (AI 4 synbio and the Mediterrain Conference on Control and Automation) and is under review at PLOS Computational Biology). 

### Software Package

The work could be released as a software package with the aim to make the implementation of the OED method accessible for use by non-experts. With a collaboration that has already been initiated we can test the package in a high throughput biological laboratory. 


## Tasks and potential roadmap
- Decide on the models we will use. These should be large scale, biologically relevant and chosen so that a range of biology is represented
- Determine if the current method of calculating optimality scales well and if required optimise this
- Determine the best way to scale up the RL and optimise
- Decide on the comparisons we will make to validate the method. These should include effectiveness, in terms of experimental optimality and parameter inference, and time taken to make decisions online
- Results/paper write up and publication
- Publish package on PyPI

## Resources

### Requirements

What kinds of resources (e.g. GPU hours, RAM, storage) are needed to complete the project?

### Timeline

6 months to 1 year

## Broader Impact

Using reinforcement leaning for optimal experimental design has compelling advantages of traditional approaches, mainly fast online decision making and the ability to easily incorporate parameter/model uncertainty. Indeed we have already been contacted by another group to implement our method in their lab, because they are struggling with the slow speed of optimisation base approaches. The extension of the method to large scale biological models and the development of an easy to use package would have wide spread impact on the design of optimal experiments in biology. Finally, the generality of the method means that it could have further impact in other fields such as the other sciences and engineering. 

## Reproducibility

All code can be published publicly on GitHub, with working examples to run on various models. Trained models could also be published. 

## Failure Case

If our findings are unsatisfactory, do we have an exit plan? Do we have deliverables along the way that we can still provide the community with?

As the effectiveness of the method has already been demonstrated. The failure case now is that the training time becomes prohibitive to use it on models that are relevant to the user with the hardware that they have available. We can still demonstrate the method and show that using the hardware we have available we can perform OED on complex biological models. The community can use it for models of a scale that their hardware would allow. 

## Preliminary Findings

We have written a [paper](https://www.biorxiv.org/content/10.1101/2022.05.09.491138v1.abstract), currently on bioArxiv and in review at PLOS computational biology which demonstrates the effectiveness of the method on simple models. 


## Next Steps

Expand the project into models other areas of science and engineering. There is also the possibility to remove the restriction to models described by PDEs. Furthermore, we could look into different experimental optimality metrics.

## Known contributors

Neythen Treloar, Postdoctoral Research Fellow, University College London
