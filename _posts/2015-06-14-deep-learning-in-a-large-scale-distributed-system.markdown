---
layout: post
title:  "Deep learning in a large scale distributed system"
date:   2015-06-14 10:39:00
tags: [machine-learning, papers, deep-learning, google, distributed-systems, distbelief]
summary: "Deep learning is interesting in many ways. But when you consider to do it in thousands of cores that can process millions of parameters, then the problem is more interesting and complex at the same time."
---

Deep learning is interesting in many ways. But when you consider to do it in thousands of cores that can process millions of parameters, then the problem is more interesting and complex at the same time.

<img src="/assets/images/datacenter.jpg" alt="" width="690" /> Google Datacenter (via Google)

Google was doing an interesting experiment, training a deep network with millions of parameters in thousands of CPUs. The goal was to train very large datasets without to limit the form of the model.

The <a title="Large Scale Distributed Deep Networks" href="http://research.google.com/archive/large_deep_networks_nips2012.html" target="_blank">paper</a> describes the use of DistBelief, a framework created for distributed parallel computing applied to deep learning training. A collection of the features that the framework manage by itself are:

> The framework automatically parallelizes computation in each machine using all available core, and
> manages communication, synchronization and data transfer between machines during both training and
> inference.

I couldn't find too much information about it, only what it is written in the paper.

They have applied two algorithms: <a href="http://en.wikipedia.org/wiki/Stochastic_gradient_descent" target="_blank">SGD</a> (Stochastic Gradient Descent) and <a href="http://en.wikipedia.org/wiki/Limited-memory_BFGS" target="_blank">L-BFGS</a>. These algorithms usually works well, but they doesn't scale with very large data sets. That is because they introduce some modifications to them. The paper gives you more details about the optimizations in both algorithms that you can find interesting.

I was found really interesting the idea of distributed parallel computing working for very large datasets  in such algorithms.

You can read <a href="http://research.google.com/archive/large_deep_networks_nips2012.html" target="_blank">"Large Scale Distributed Deep Networks"</a>, or if you are interested in the <a href="http://static.googleusercontent.com/media/research.google.com/en//archive/large_deep_networks_nips2012.pdf" target="_blank">pdf version</a>. Have fun!
