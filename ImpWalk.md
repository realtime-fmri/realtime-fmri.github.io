---
layout : page
title : Implementation Walkthough
subtitle : 
order : 1
---
## Existing real-time fMRI implementations

There are a variety of ways one can extract fMRI information based on how the brain is responding during an experiment, and then
 use this information to change stimuli (neurofeedback) or controll brain computer interfaces (BCI).  
The majority of real-time fMRI has focused on the use of univariate statistical analysis approaches related to the general linear model
(GLM) [\(Friston et al., 1995b\)](http://spin.ecn.purdue.edu/fmri/PDFLibrary/FristonK_HBM_1995_2_189_210.pdf) or to tracking the 
fMRI signal in one or a few regions of interest (ROIs). However, there are also real-time fMRI approaches that predict brain-states for feedback using distributed brain-state patterns. In other words, it's an approach of brain reading rather than that of localized activation.

In this section we will walkthough the different ways of implementing real-time fMRI.




##Univariate statistical approaches


### Region Of Interest (ROI)


Turbo BrainVoyager



##  Brain state prediction real-time fMRI.


### Temporally Adaptive Brain State (TABS) fMRI.

This part describes brain-state prediction real-time fMRI from [\(LaConte et al., 2007,](http://www.ncbi.nlm.nih.gov/pubmed/17133383)[ 2011\)] (http://www.ncbi.nlm.nih.gov/pubmed/?term=Decoding+fMRI+brain+states+in+real-time+laConte)

Therea are several advantages of brain-state prediction real-time fMRI. The first advantage is that prior assumptions
 about functional localization and individual performance strategies are not required-the system learns these directly from the volunteer. This provides
for a high degree of experimental flexibility across the spectrum of cognitive domains. The second advantage
is that feedback can rely on a direct, intuitive translation of brain state, rather than a representation based on
increasing or decreasing local activity. The potential benefit to fMRI research is quite high, as this approach provides
the capability for a new class of experimental designs in which real-time feedback control of the stimulus
is possible—rather than using a fixed paradigm, experiments can adaptively evolve as subjects receive
brain-state feedback.





The minimum required equipment that you will need to run a powerfull rt-fMRI on your scanner could look something like this:

CPU
RAM
etc.. 


