---
title: Research Interests
feature_image: "https://github.com/EncisoAlva/EncisoAlva.github.io/blob/main/img/banner_tulip.jpg?raw=true"
---

Electrical Source Imaging (ESI) is a technique used to identify neural sources of electrical activity inside the brain, which may be related to normal or pathological states, given recordings of surface electric potentials like [EEG](https://en.wikipedia.org/wiki/Electroencephalography)). 
Applications of ESI include Neuropsychology and non-invasive monitoring of Epileptogenesis, among others.

![Inverse problem of Electric Source Imaging, simplified.](https://github.com/EncisoAlva/EncisoAlva.github.io/blob/main/img/InverseProblemESI.png?raw=true)

The mathematical formulation of this task includes solving the system 

$$ \mathbf{G}\, {\color{red} \mathbf{S}} + \varepsilon = \mathbf{Y} $$

for ${\color{red} \mathbf{S}}$, given $\mathbf{Y}$ and $\mathbf{G}$ an $m\times n$ matrix with $m\ll n$; usually $m\approx \mathcal{O}(100)$ and $m\approx \mathcal{O}(1,000)$.
The details of such formulation are very interesting. 
I personally recommend reading [this book](https://academic.oup.com/book/2998) book of Nunez and Srinavasan or [this paper](https://jneuroengrehab.biomedcentral.com/articles/10.1186/1743-0003-4-46) from Hallez.

This equation clearly don't have an unique solution for ${\color{red} \mathbf{S}}$... unless we get more information from the context.
* Minimal-norm models assume that ${\mathbf{S}}$ has a small norm. Some authors use $\ell_2$ or $\ell_1$ norm, even $\ell_{1,2}$ norm. Maybe the norm of the total variation of ${\mathbf{S}}$ over time or space.
* Multi-modal models use information obtained from _other_ types of data: CT, fMRI, NIRS, PET, etc.

An effective and fast solution of this problem requires using Convex Optimization, either smooth or non-smooth, as well as Numerical Methods.

* Non-invasive monitoring of ictal activity in infants.
  * Using ESI from EEG data, the activity from certain brain areas during ictal activity was explored. 
  * Subjects were infants with Glut1 deficiency.
  * Results from this analysis were included in a collaborative paper [(link)](https://www.science.org/doi/10.1126/scitranslmed.abn2956).
* Evaluation of multi-modal ESI methods from EEG.
  * ESI methods were modified to include information from fMRI to increase accuracy.
  * Results from this process were presented as a [poster](/files/AIMSposter230528.pdf?raw=true).
* Evaluation of Virtual Deep Electrodes from ESI data.
  * ESI data was used to estimate the measurements from hypothetical electrodes inserted inside the brain, referred to as Virtual Electrodes.
  * Virtual Electrodes were compared with recordings from electrodes inserted in the brain.
  * The technology of Virtual Electrodes is quite recent, this may be the first study of stroke using them.
  * Manuscript under review.
* Novel ESI methods based on multi-modal priors.
  * ESI methods were modified (again) to include information from pathology to increase accuracy.
  * Multiple spatial priors can be used to boost the accuray of ESI.
  * Some preliminary results were presented using [these slides](/files/EncisoAlva_240226.pdf?raw=true) and [this poster](/files/Mathposium23_EncisoAlva.pdf?raw=true).
  * Officially, this is my dissertation topic.
* Novel ESI methods from Dura Imaging and Neural Networks.
  * Dura Imaging (DI) estimates the electric potential through the dura before reaching the scalp electrodes. 
  * DI was used as intermediary for ESI with the aid of artificial neural networks.
  * Not my dissertation, because it is a very recent idea.

