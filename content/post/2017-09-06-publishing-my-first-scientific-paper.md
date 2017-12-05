---
title: Publishing my first scientific paper
author: ~
date: '2017-09-06'
#image: "post/2hc.mp4"
slug: publishing-my-first-scientific-paper
categories: []
tags: [compchem]
---
At the end of 2016, [Rachel Crespo-Otero](https://crespootero.wordpress.com/) and I received news that our submitted manuscript was to be published in the journal *Physical Chemistry Chemical Physics*. It was a great piece of news to receive before the Christmas holidays and was met with both joy and relief. It was the culmination of 12 months of work - the manuscript had taken many guises before we were happy enough to submit. This was my first scientific publication and in this post I want to give some background into the project, how we approached the problem, and the process of publishing in a peer-reviewed academic journal.

In our group, we are interested in modelling the photochemistry of molecules which undergo some kind of ‘switching’ process when they absorb light, for use in photochromic materials. In October 2015, we were intrigued by photochromes based on 2’-hydroxychalones. When exposed to UV-light, these systems undergo excited state intramolecular proton transfer (ESIPT), a highly interesting and useful phenomenon which can be used in optoelectronics, imaging, and solid state lasers. Essentially, the substance absorbs UV light, and emits (fluoresces) red light. Crucially, the fluorscence only occurs in the solid state. When in solution, there is no light emission. We were interested in studying the mechanism for how the molecule emits light in the solid state, but not in solution. 

The project would involve two stages. The aim of the first part was to model why there is no fluorescence in the gas/liquid phase. Once that was established, we would model the fluorescence in the solid state. Without getting too technical, when a molecule is irradiated by UV light, this energy is used to promote, or *excite*, an electron into a higher energetic state. In stage one, presented in the paper, we modelled how this process happens in this system, and then how the molecule *relaxes* back to the lowest energy ground state. 

As discussed in the paper, we uncover two relaxation channels in the first excited state (S1) which cause the S0 and S1 states to converge. We studied how different molecular groups and their position influence each pathway and the qualitative timeframe in which proton transfer can occur (**fast** - ~50 femtoseconds). The proton transfer is visualised below. The bottom plot shows the energy difference between the two states, and approaches zero after proton transfer - determined by the intersecton of red and blue lines in top plot).

![my-image](/img/2hc.gif)

Whenever I read a paper in the literature, it appears that all of the pieces fell beautifully in to place for the authors and the final product reflects exactly how the work was carried out. I have now learned first-hand that this is (almost never) the case. In January 2015, I started writing the paper thinking that I already had most of the data. In fact, it took another six months of calculations to finally complete the picture. The most time-consuming (and frustrating) part was understanding the effect of method, as nothing seemed to match in the beginning. It was only through really understanding the strengths and limitations of each method did the data make sense.

The most enjoyable part was the running and analysis of the dynamics calculations. I used Jupyter notebooks with python/matplotlib to interpret the data, which allowed me to write scripts to analyse and plot on-the-fly.  It was a workflow which was really efficient, as a slight modification to the analysis codes could easily produce new figures, something I was thankful for upon returning to the data ~4 months later to respond to the reviewers’ questions. 

The review process itself was better than I expected - I have heard some horror stories about [reviewer 3](https://twitter.com/thirdreviewer?lang=en). For the most part, they understood the paper and what we were trying to communicate. We clarified some sections and made the manuscript a bit slicker and tighter. They didn't fully understand our analysis of the dynamics data, so I had to make some of the plots more simple and illustrative. In the end I think it was for the best. After our revisions, it was accepted by the editor. 

Going forward, we are almost ready to publish the paper for the second step of this study. We have lots of data which I have been collecting and analysing over the last 5 months or so. It should produce a really good paper once the final holes are filled in.

md







