---
title: Research Interests
feature_image: "https://github.com/EncisoAlva/EncisoAlva.github.io/blob/main/img/banner_tulip.jpg?raw=true"
---

This part is under constant updates. I'm more a fan of visual than of words. Please check [these slides](/files/EncisoAlva_240226.pdf?raw=true) about my research, they were planned for a 3 minutes presentation.

...

On general terms, my current research is based on finding solutions to matrix equations similar to the following,

$$ \mathbf{G}\, {\color{red} \mathbf{S}} = \mathbf{Y} $$

where $\mathbf{G}$ is a $m\times n$ matrix with $m \ll n$; take for example $m\approx 100$ and $n\approx 2,000$. This equation clearly don't have an unique solution for ${\color{red} \mathbf{S}}$... unless we get more information from the context.

Equation (1) arises in numerous scenarios. One of those is Electrical Source Imaging (ESI): the electrical potential fields on the scalp, measured using [EEG](https://en.wikipedia.org/wiki/Electroencephalography)), is originated the superimposed poststinaptic potentials from all the neurons inside the brain.
The ESI model all those neuron potentials as a scalar potential field, which is approximated by a finite number of dipoles with known location.

For a quick summary, ESI approximates the neural electric activity using some dipoles; larger magnitude means more measurable electric activity.


If it is assumed that the dipoles’ position is known and fixed, then the relation between the unknown dipoles’ magnitude (J) and the EEG recordings (Y) is linear as in equation (1). The mixing operator G is constructed by solving –numerically– a Laplace partial differential equation for each dipole, with the geometric domain of the subject’s head. Further details are not included in this document; they can be consulted elsewhere –for instance, in the review from Hallez [3]. 


...

Electrical Source Imaging (ESI) is a family of methods for estimating the location of neural electrical sources inside the brain, based on recordings from electrodes located either at the scalp (EEG), brain cortex (ECoG), or stylets inside the brain (SEEG). Applications of ESI include non-invasive detection of epileptogenic zones.  

Electrode recordings are known to have a high resolution in time and a poor resolution in space, and ESI inherits these characteristics. The inclusion of additional modalities of data, such as fMRI, could be integrated in the ESI formulation to increase its resolution, speed, and robustness to noise. 

Novel applications of ESI include Virtual Electrodes (VEs): estimates for recordings from inserted electrodes which are computed from ESI data. VEs are relatively inexpensive and non-intrusive in comparison with inserted electrodes, and their characteristics and limitations are similar as the data modalities they're based on.  

My current research is focused on generating better multi-modal ESI methods, optimized for clinical applications and its requirements –better resolution, more robustness to noise, improved speed, etc.  

Past research projects are listed below:
* Novel ESI methods with regional Bayesian priors, with applications to Virtual Electrodes. 
* Evaluation of fMRI-informed EEG-based ESI techniques. 
* Validation of ESI techniques from ECoG data in a pig model. 
* ESI from EEG during epilepsy on infants. 
