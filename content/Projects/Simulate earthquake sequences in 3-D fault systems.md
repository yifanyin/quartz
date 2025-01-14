---
title: "Simulate earthquake sequences in 3-D fault systems"
tags:
- project
- simulation
- seismicity
---
How to create a [[Modeling earthquakes|synthetic seismic sequence]]? Surely one can use the statistics to generate one. But we know plates move and faults slide. How do we incorporate these information when generating sequences?

The statistical route of generating synthetic seismicity is using the [[ETAS]] (epidemic-type aftershock sequence) model. ETAS relies on the scaling-law parameters that are fitted to real catalogs. Another more physical route is the cellular automata models commonly called the earthquake simulators. The earthquake simulators takes the fault geometries as the model mesh and simulate patch sliding and interactions just like what we imagine earthquakes do. Because the failure criterion is as simple as on-off switches, these models are very efficient for models with large degrees of freedom and a long simulated period. Better still, the event generated reproduce the power-law magnitude distribution seen in earthquake catalogs. But because the failure mechanisms are simple, the simulators do not recover the details of nucleation, propagation and finally arrest. The models that can do so solves the conservation equations using various numerical methods. These class of models are capable to reproduce rupture processes and even ground motions. However, they are computationally demanding, especially for multiple earthquake cycles. 

Is there a way for us greedy scientists to have both phenomena in one simulation? A model that solves the differential equations but also produces diverse events that compose frequency-magnitude distribution? In this project we achieve such simulations using appropriate frictional parameters, fault interactions, and a suitable solver to vastly improve the time-stepping efficiency of [[QDYN]], a rupture simulator. The result is a simple fault system that generate diverse earthquake sequence.

![[pap2_tweet.gif]]

Our result shows that with fault interaction that naturally exists within the crust, it's a lot easier to generate earthquake sequences that resemble real sequences, albeit that the maximum magnitude is bounded by the fault size. There are other factors we have yet to put in the model, such as heterogeneous frictional properties and non-planar fault planes. The result gives us chances to exam the effect of all these factors that create the statistical signatures of seismicity as we know it.

# Perspectives
- #Question What does the distribution look like for seismicity generated on the same fault? Are they characteristic in sizes? Are they more or less repetitive in time?
    -  Yan Y. Kagan, David D. Jackson, Robert J. Geller; **Characteristic Earthquake Model, 1884–2011, R.I.P.**. *Seismological Research Letters* 2012; 83 (6): 951–953. doi: [10.1785/0220120107](https://doi.org/10.1785/0220120107](https://doi.org/10.1785/0220120107)
    - [[Magnitude-frequency distribution#The moment-frequency relations|General MFDs]]

# Publication
- **Yin, Y.**, Galvez, P., Heimisson, E. R., & Wiemer, S. (2023). The role of three-dimensional fault interactions in creating complex seismic sequences. _Earth and Planetary Science Letters_, _606_(118056), 118056, doi: [10.1016/j.epsl.2023.118056](https://doi.org/10.1016/j.epsl.2023.118056)
- AGU2023 Invited talk