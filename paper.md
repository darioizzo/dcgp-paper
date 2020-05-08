---
title: 'dcgp: Differentiable Cartesian Genetic Programming made easy.'
tags:
  - Python
  - genetic programming
  - cartesian genetic programming
  - symblic regression
  - neural networks
authors:
  - name: Dario Izzo
    orcid: 0000-0002-9846-8423
    affiliation: 1
  - name: Francesco Biscani
    affiliation: 2
affiliations:
 - name: Advanced Concepts Team, European Space Research and Technology Center (Noordwijk, NL)
   index: 1
 - name: Max Planck Institute for Astronomy (Heidelberg, D)
   index: 2
date: 5 May 2020
bibliography: paper.bib
---

# Summary

Genetic Programming (GP), is a computer technique based on the idea of representing computer programs as some sort of tree (data-structure) and
evolving it using genetic algorithms, as to improve the programs *fitness* at solving a predefined task. The idea flourished in the late 80s mainly thanks to the work of John Koza [@koza:2017], and has always had a major *skeleton in the closet* (to use the words of Koza): the difficulty to find and evolve real valued parameters in the expressed programs. The recent development called **differentiable
genetic programming** [@izzo:2017], was introduced to address exactly this issue and allows to learn constants in computer programs using the
differential information of the loss associated to the program as obtained using automated differentiation techniques. 

The evolution of a **differentiable genetic program** can be supported by using the information on the derivatives of the program outputs with respect to chosen parameters, enabling in GP the equivalent of back-propagation in Artificial Neural Networks (ANN). The fitness of a program can thus be defined in terms of the derivatives, allowing to go beyond symbolic regression tasks and, for example, to solve differential equations, learn differential models, capture conserved quantities in dynamical systems, search for Lyapunov functions in controlled systems, etc..

# References